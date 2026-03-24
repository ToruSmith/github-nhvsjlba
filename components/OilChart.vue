<template>
  <div style="position:relative; width:100%; height:300px;">
    <canvas ref="canvasRef"></canvas>
  </div>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue'
import {
  Chart,
  LineController, LineElement, PointElement,
  LinearScale, CategoryScale,
  Filler, Tooltip, Legend
} from 'chart.js'

Chart.register(
  LineController, LineElement, PointElement,
  LinearScale, CategoryScale,
  Filler, Tooltip, Legend
)

const canvasRef = ref(null)
let chartInstance = null

onMounted(() => {
  if (!canvasRef.value) return
  chartInstance = new Chart(canvasRef.value, {
    type: 'line',
    data: {
      labels: ['2/27','3/1','3/2','3/4','3/6','3/8','3/9','3/11','3/13','3/15','3/18','3/20','3/21','3/23'],
      datasets: [
        {
          label: '布蘭特原油 (USD/桶)',
          data: [73, 80, 82, 87, 96, 103, 120, 92, 100, 97, 110, 112, 106, 100],
          borderColor: '#c0392b',
          backgroundColor: 'rgba(192,57,43,0.08)',
          tension: 0.4,
          fill: true,
          pointRadius: 5,
          pointHoverRadius: 9,
          borderWidth: 2.5,
        },
        {
          label: 'WTI 原油 (USD/桶)',
          data: [67, 73, 75, 80, 88, 95, 119, 87, 95, 91, 103, 105, 98, 88],
          borderColor: '#2980b9',
          backgroundColor: 'transparent',
          tension: 0.4,
          fill: false,
          borderDash: [5, 4],
          pointRadius: 3,
          borderWidth: 2,
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
            label: (ctx) => `${ctx.dataset.label}: $${ctx.parsed.y}/桶`
          }
        }
      },
      scales: {
        x: { grid: { color: 'rgba(0,0,0,0.05)' } },
        y: {
          min: 60, max: 130,
          ticks: { callback: (v) => '$' + v },
          grid: { color: 'rgba(0,0,0,0.05)' }
        }
      }
    }
  })
})

onBeforeUnmount(() => {
  chartInstance?.destroy()
})
</script>
