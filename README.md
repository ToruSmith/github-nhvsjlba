# 2026 美伊戰爭近況與台灣因應策略 — Slidev 簡報 v2

## 📦 專案結構

```
iran-briefing-v2/
├── package.json          ← 釘版號，StackBlitz 穩定用
├── slides.md             ← 主要簡報（15頁，無 script setup）
├── components/
│   ├── OilChart.vue      ← 布蘭特 vs WTI 折線圖
│   ├── EnergyChart.vue   ← 台灣能源曝險雙軸圖
│   ├── HeChart.vue       ← 氦氣來源圓環圖（台灣 vs 韓國）
│   └── ScenarioBar.vue   ← 貝氏情境機率雙軸柱狀圖
└── README.md
```

---

## 🚀 StackBlitz 操作步驟

### 上傳方式（最穩定）

1. 開啟 [stackblitz.com](https://stackblitz.com) → **New Project** → **Node.js**
2. 刪除預設所有檔案
3. 重建以下資料夾結構，並貼入各檔案內容：
   - `package.json`
   - `slides.md`
   - `components/OilChart.vue`
   - `components/EnergyChart.vue`
   - `components/HeChart.vue`
   - `components/ScenarioBar.vue`
4. StackBlitz Terminal 輸入：
   ```bash
   npm install && npm run dev
   ```

> ⚠️ v2 版本改為元件化架構，修正 `RangeError: failed to grow memory` 問題。
> 根本原因：單一 slides.md 內不可有多個 `<script setup>` 區塊。

---

## 💻 本機執行（Node.js 18+）

```bash
npm install
npm run dev
```

若仍發生記憶體不足：
```bash
node --max-old-space-size=4096 ./node_modules/.bin/slidev slides.md
```

---

## ✨ Slidev 互動功能清單

| 功能 | 位置 |
|------|------|
| `v-click` 逐步揭露 | 幾乎所有頁面 |
| `v-clicks` 批次動畫 | 第3頁時間軸 |
| Chart.js 互動懸停 Tooltip | 第7、10、11、12頁 |
| Chart.js `onBeforeUnmount` 記憶體釋放 | 所有4個元件 |
| KaTeX 數學公式渲染 | 第8、12頁 |
| 程式碼逐段高亮 `{all｜1-8｜10-16｜18-24}` | 第8頁 |
| YouTube iframe 嵌入 | 第6頁 |
| `two-cols` 雙欄佈局 | 第2、4、5、13、15頁 |
| 多種 transition 動畫 | 全頁 |
| 自訂 CSS 元件（`.nb`、`.wb`、`.kpi`、`.tag-*`） | 全頁 |

---

## ⚠️ YouTube 影片替換

第6頁影片目前為佔位符，請替換 `slides.md` 中：

```
src="https://www.youtube.com/embed/dQw4w9WgXcQ?rel=0"
```

建議來源：
- [Al Jazeera English](https://www.youtube.com/@AlJazeeraEnglish) — 搜尋 "Strait of Hormuz 2026"
- [BBC News](https://www.youtube.com/@BBCNews) — 搜尋 "Iran war March 2026"

YouTube 影片 ID 位於網址 `?v=` 後方。

---

## 📋 資料截止與免責聲明

- 資料截止：**2026年3月24日**
- 統計推估（波動率、情境機率）基於公開數據，非官方機構正式預測
- 供機關內部決策參考，不代表任何政治立場
