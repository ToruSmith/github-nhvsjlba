<template>
  <div style="position:relative; width:100%; height:280px;">
    <canvas ref="canvasRef"></canvas>
  </div>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue'
import {
  Chart,
  BarController, BarElement,
  LineController, LineElement, PointElement,
  LinearScale, CategoryScale,
  Tooltip, Legend
} from 'chart.js'

Chart.register(
  BarController, BarElement,
  LineController, LineElement, PointElement,
  LinearScale, CategoryScale,
  Tooltip, Legend
)

const canvasRef = ref(null)
let chartInstance = null

onMounted(() => {
  if (!canvasRef.value) return
  chartInstance = new Chart(canvasRef.value, {
    data: {
      labels: ['石油', 'LNG（天然氣）', '煤炭'],
      datasets: [
        {
          type: 'bar',
          label: '途經荷莫茲比例 (%)',
          data: [72, 28, 8],
          backgroundColor: [
            'rgba(192,57,43,0.8)',
            'rgba(214,137,16,0.8)',
            'rgba(41,128,185,0.5)'
          ],
          borderColor: ['#c0392b','#d68910','#2980b9'],
          borderWidth: 2,
          yAxisID: 'y',
        },
        {
          type: 'line',
          label: '安全存量（天）',
          data: [90, 11, 30],
          borderColor: '#1a5276',
          backgroundColor: 'transparent',
          pointRadius: 8,
          pointStyle: 'rectRot',
          borderWidth: 2.5,
          yAxisID: 'y2',
        }
      ]
    },
    options: {
      responsive: true,
      maintainAspectRatio: false,
      interaction: { mode: 'index', intersect: false },
      plugins: {
        legend: { position: 'top' },
        tooltip: {
          callbacks: {
            label: (ctx) => ctx.datasetIndex === 0
              ? `荷莫茲曝險：${ctx.parsed.y}%`
              : `安全存量：${ctx.parsed.y} 天`
          }
        }
      },
      scales: {
        y: {
          type: 'linear', position: 'left',
          max: 100, min: 0,
          ticks: { callback: (v) => v + '%' },
          title: { display: true, text: '荷莫茲依賴比例 (%)' }
        },
        y2: {
          type: 'linear', position: 'right',
          max: 100, min: 0,
          ticks: { callback: (v) => v + '天' },
          title: { display: true, text: '安全存量（天）' },
          grid: { drawOnChartArea: false }
        }
      }
    }
  })
})

onBeforeUnmount(() => {
  chartInstance?.destroy()
})
</script>
