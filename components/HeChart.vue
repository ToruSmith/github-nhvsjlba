<template>
  <div style="position:relative; width:100%; height:260px;">
    <canvas ref="canvasRef"></canvas>
  </div>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue'
import {
  Chart,
  DoughnutController, ArcElement,
  Tooltip, Legend
} from 'chart.js'

Chart.register(DoughnutController, ArcElement, Tooltip, Legend)

const canvasRef = ref(null)
let chartInstance = null

onMounted(() => {
  if (!canvasRef.value) return
  chartInstance = new Chart(canvasRef.value, {
    type: 'doughnut',
    data: {
      labels: [
        '🇹🇼 卡達 30%',
        '🇹🇼 美國 30%',
        '🇹🇼 其他 40%',
        '🇰🇷 卡達 80%',
        '🇰🇷 其他 20%'
      ],
      datasets: [
        {
          label: '台灣氦氣來源',
          data: [30, 30, 40, 0, 0],
          backgroundColor: ['#c0392b','#2980b9','#1e8449','transparent','transparent'],
          hoverOffset: 12,
          borderWidth: 2,
        },
        {
          label: '韓國氦氣來源',
          data: [0, 0, 0, 80, 20],
          backgroundColor: ['transparent','transparent','transparent','#e74c3c','#aab7b8'],
          hoverOffset: 12,
          borderWidth: 2,
        }
      ]
    },
    options: {
      responsive: true,
      maintainAspectRatio: false,
      plugins: {
        legend: {
          position: 'right',
          labels: { font: { size: 11 }, filter: (item) => item.text.trim() !== '' }
        },
        tooltip: {
          filter: (item) => item.parsed > 0,
          callbacks: {
            label: (ctx) => {
              const ring = ctx.datasetIndex === 0 ? '台灣' : '韓國'
              return `${ring}：${ctx.label} → ${ctx.parsed}%`
            }
          }
        }
      },
      cutout: '45%'
    }
  })
})

onBeforeUnmount(() => {
  chartInstance?.destroy()
})
</script>
