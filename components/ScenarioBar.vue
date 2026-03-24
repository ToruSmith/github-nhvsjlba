<template>
  <div style="position:relative; width:100%; height:200px;">
    <canvas ref="canvasRef"></canvas>
  </div>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue'
import {
  Chart,
  BarController, BarElement,
  LinearScale, CategoryScale,
  Tooltip, Legend
} from 'chart.js'

Chart.register(BarController, BarElement, LinearScale, CategoryScale, Tooltip, Legend)

const canvasRef = ref(null)
let chartInstance = null

onMounted(() => {
  if (!canvasRef.value) return
  chartInstance = new Chart(canvasRef.value, {
    type: 'bar',
    data: {
      labels: ['A：快速停火（3/28前）', 'B：長期對峙（4月以上）', 'C：衝突升級'],
      datasets: [
        {
          label: '貝氏更新後機率 (%)',
          data: [35, 45, 20],
          backgroundColor: ['#1e8449','#d68910','#c0392b'],
          borderRadius: 6,
          borderWidth: 0,
        },
        {
          label: '台灣GDP衝擊 (負值 %)',
          data: [0.3, 0.8, 1.5],
          backgroundColor: ['rgba(30,132,73,0.3)','rgba(214,137,16,0.3)','rgba(192,57,43,0.3)'],
          borderRadius: 6,
          borderWidth: 1,
          borderColor: ['#1e8449','#d68910','#c0392b'],
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
              ? `情境機率：${ctx.parsed.y}%`
              : `GDP衝擊：−${ctx.parsed.y}%`
          }
        }
      },
      scales: {
        y: {
          max: 60, min: 0,
          ticks: { callback: (v) => v + '%' },
          title: { display: true, text: '情境機率 (%)' }
        },
        y2: {
          type: 'linear', position: 'right',
          max: 2, min: 0,
          ticks: { callback: (v) => '−' + v + '%' },
          title: { display: true, text: 'GDP衝擊' },
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
