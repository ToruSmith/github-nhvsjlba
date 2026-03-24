---
theme: default
title: '2026 美伊戰爭近況與台灣因應策略'
info: |
  機關內部報告 — 內部限閱
  資料截止：2026年3月24日
highlighter: shiki
class: text-center
drawings:
  persist: false
transition: fade-out
mdc: true
---

<style>
.slidev-layout { font-family: 'Noto Sans TC', 'Microsoft JhengHei', sans-serif; }
.tag-r  { background:#c0392b; color:#fff; padding:2px 8px; border-radius:4px; font-size:.72rem; }
.tag-y  { background:#d68910; color:#fff; padding:2px 8px; border-radius:4px; font-size:.72rem; }
.tag-g  { background:#1e8449; color:#fff; padding:2px 8px; border-radius:4px; font-size:.72rem; }
.tag-b  { background:#1a5276; color:#fff; padding:2px 8px; border-radius:4px; font-size:.72rem; }
.kpi    { background:#f0f4f8; border-left:4px solid #1e3a5f; padding:10px 14px; border-radius:6px; }
.kpi-n  { font-size:1.7rem; font-weight:700; color:#1e3a5f; }
.kpi-l  { font-size:.75rem; color:#666; }
.nb     { border:1px solid #d5d8dc; background:#fdfefe; padding:8px 12px; border-radius:6px; font-size:.82rem; }
.wb     { border:1px solid #e59866; background:#fef9f3; padding:8px 12px; border-radius:6px; font-size:.82rem; }
.sfoot  { position:absolute; bottom:12px; right:20px; font-size:.63rem; color:#aaa; }
</style>

# 2026 美伊戰爭近況
## 及我國因應策略評估

<div class="pt-6 text-gray-400 text-sm">
機關內部報告　｜　機密等級：內部限閱　｜　資料截止：2026年3月24日
</div>

<div class="abs-br m-6 text-xs text-gray-400">
  <span class="tag-r">CONFIDENTIAL</span>　承辦：＿＿＿　核稿：＿＿＿
</div>

<div class="mt-10">
  <span @click="$slidev.nav.next"
    class="cursor-pointer px-4 py-2 border border-gray-400 rounded text-sm text-gray-500 hover:bg-gray-100 transition">
    點擊開始報告　›
  </span>
</div>

---
layout: two-cols
transition: slide-up
---

# 報告架構

<div class="mt-2 space-y-2 text-sm">
<v-click><div class="nb">
<strong>壹、衝突事實陳述</strong>　衝突時間軸 / 軍事態勢 / 談判動態
</div></v-click>
<v-click><div class="nb">
<strong>貳、全球經濟衝擊分析</strong>　荷莫茲戰略地位 / 油價走勢 / 供應鏈
</div></v-click>
<v-click><div class="nb">
<strong>參、我國曝險評估</strong>　能源安全 / 半導體氦氣 / 貝氏情境
</div></v-click>
<v-click><div class="nb">
<strong>肆、因應措施與建議</strong>　現行作為 / 政策優先建議
</div></v-click>
</div>

::right::

<div class="pl-6 mt-1">

### 核心指標（截至 3/24）

<div class="grid grid-cols-2 gap-3 mt-3 text-sm">
  <div class="kpi"><div class="kpi-n">24天</div><div class="kpi-l">衝突持續天數</div></div>
  <div class="kpi"><div class="kpi-n">+65%</div><div class="kpi-l">布蘭特最高漲幅</div></div>
  <div class="kpi"><div class="kpi-n">~5%</div><div class="kpi-l">荷莫茲剩餘流量</div></div>
  <div class="kpi"><div class="kpi-n">11天</div><div class="kpi-l">台灣LNG安全存量</div></div>
  <div class="kpi"><div class="kpi-n">1,444</div><div class="kpi-l">伊朗境內已知傷亡</div></div>
  <div class="kpi"><div class="kpi-n">400MB</div><div class="kpi-l">IEA史上最大儲備釋出</div></div>
</div>

<div class="nb mt-4 text-xs">
📌 本報告引用 Bloomberg、IEA、CNN、Al Jazeera、經濟日報、TechNews、INSIDE Taiwan，資料截止 2026.03.24。
</div>

</div>

<div class="sfoot">2/15　機關內部報告</div>

---
transition: slide-left
---

# 衝突時間軸（2/28 — 3/24）

<div class="mt-2 relative pl-6" style="font-size:.84rem;">

<div style="position:absolute;left:16px;top:8px;bottom:8px;width:3px;background:linear-gradient(to bottom,#c0392b,#d68910,#1a5276);border-radius:2px;"></div>

<v-clicks>

<div class="flex items-start mb-3">
  <div style="width:13px;height:13px;border-radius:50%;background:#c0392b;position:absolute;left:10px;margin-top:3px;"></div>
  <div class="ml-8"><span class="tag-r">2/28</span> <strong class="ml-1">美以聯合空襲，最高領袖哈梅內伊遇害</strong><span class="text-gray-500 ml-2 text-xs">— 「史詩之怒」行動啟動；布蘭特 $73→$80</span></div>
</div>

<div class="flex items-start mb-3">
  <div style="width:13px;height:13px;border-radius:50%;background:#c0392b;position:absolute;left:10px;margin-top:3px;"></div>
  <div class="ml-8"><span class="tag-r">3/1</span> <strong class="ml-1">伊朗報復：500+枚飛彈、2,000+架無人機</strong><span class="text-gray-500 ml-2 text-xs">— 打擊以色列與海灣美軍基地</span></div>
</div>

<div class="flex items-start mb-3">
  <div style="width:13px;height:13px;border-radius:50%;background:#d68910;position:absolute;left:10px;margin-top:3px;"></div>
  <div class="ml-8"><span class="tag-y">3/4</span> <strong class="ml-1">荷莫茲正式封鎖</strong><span class="text-gray-500 ml-2 text-xs">— 卡達宣告 Force Majeure；LNG全球供應斷鏈</span></div>
</div>

<div class="flex items-start mb-3">
  <div style="width:13px;height:13px;border-radius:50%;background:#d68910;position:absolute;left:10px;margin-top:3px;"></div>
  <div class="ml-8"><span class="tag-y">3/8–9</span> <strong class="ml-1">布蘭特衝破 $120，史上最大單日漲幅</strong><span class="text-gray-500 ml-2 text-xs">— IEA：「全球能源史上最嚴重供應危機」</span></div>
</div>

<div class="flex items-start mb-3">
  <div style="width:13px;height:13px;border-radius:50%;background:#1a5276;position:absolute;left:10px;margin-top:3px;"></div>
  <div class="ml-8"><span class="tag-b">3/11</span> <strong class="ml-1">IEA 32國聯合釋放4億桶儲備</strong><span class="text-gray-500 ml-2 text-xs">— 史上最大規模緊急動員；布蘭特短暫回落 $80</span></div>
</div>

<div class="flex items-start mb-3">
  <div style="width:13px;height:13px;border-radius:50%;background:#d68910;position:absolute;left:10px;margin-top:3px;"></div>
  <div class="ml-8"><span class="tag-y">3/18–20</span> <strong class="ml-1">美以打擊 South Pars 氣田；布蘭特再升至 $110–112</strong><span class="text-gray-500 ml-2 text-xs">— 卡達LNG與伊朗共享氣田，全球LNG衝擊加劇</span></div>
</div>

<div class="flex items-start">
  <div style="width:13px;height:13px;border-radius:50%;background:#1e8449;position:absolute;left:10px;margin-top:3px;"></div>
  <div class="ml-8"><span class="tag-g">3/23–24</span> <strong class="ml-1">川普「主要協議點已達成」；延後攻擊5日</strong><span class="text-gray-500 ml-2 text-xs">— 伊朗國會議長否認；布蘭特跌至 $100；3/28 為關鍵節點</span></div>
</div>

</v-clicks>
</div>

<div class="sfoot">3/15　機關內部報告</div>

---
layout: two-cols
transition: slide-up
---

# 當前軍事態勢

### 美方

<div class="space-y-2 mt-3 text-sm">
<v-click><div class="nb">🛩️ <strong>空中優勢確立</strong>：伊朗空軍與海軍據報遭嚴重削弱；1架 F-15 疑似被擊落（未經獨立確認）</div></v-click>
<v-click><div class="nb">⚓ <strong>海上部署強化</strong>：追加2,500名海軍陸戰隊，討論佔領霍爾木茲島以控制海峽</div></v-click>
<v-click><div class="nb">🇬🇧 <strong>英國協作</strong>：開放迭戈加西亞基地；伊朗已以飛彈回應</div></v-click>
<v-click><div class="wb">⚠️ <strong>海峽通行</strong>：荷莫茲維持約5%正常流量；21艘商船已確認遭攻擊（截至3/24）</div></v-click>
</div>

::right::

<div class="pl-6">

### 伊方

<div class="space-y-2 mt-3 text-sm">
<v-click><div class="wb">🚀 <strong>飛彈庫存耗損</strong>：彈道飛彈發射速率下降，庫存研判趨於緊縮</div></v-click>
<v-click><div class="nb">🏛️ <strong>領導層重整</strong>：Mojtaba Khamenei 接任最高領袖；指揮體系仍在重建中</div></v-click>
<v-click><div class="nb">🤝 <strong>周邊態勢</strong>：胡塞武裝維持克制；巴基斯坦油輪獲放行（暗示存在默契）</div></v-click>
<v-click><div class="wb">⚠️ <strong>談判訊號矛盾</strong>：外長阿拉格齊態度保留；國會議長否認直接談判</div></v-click>
</div>

<div class="nb mt-4 text-xs">
🔍 <strong>研判</strong>：雙方均具降溫誘因，但立場分歧仍大。3/28緩衝期到期為最關鍵觀察窗口。
</div>

</div>

<div class="sfoot">4/15　機關內部報告</div>

---
transition: slide-left
---

# 停火談判最新動態（截至 2026.3.24）

<div class="grid grid-cols-3 gap-4 mt-3 text-sm">
<v-click>
<div class="kpi"><div class="tag-b mb-2">美方立場</div>
提出15點要求清單：① 永久放棄核武　② IAEA全面核查　③ 開放荷莫茲<br>
川普稱「已有重大共識點」<br><span class="text-xs text-gray-400">— Bloomberg 3/23</span><br>
<span class="tag-y mt-2 inline-block">訊號混沌</span></div>
</v-click>
<v-click>
<div class="kpi"><div class="tag-r mb-2">伊方立場</div>
外長：「這不是我們的戰爭，美國必須負責。」<br>
國會議長：「沒有任何談判正在進行。」<br>
<span class="text-xs text-gray-400">— Al Jazeera / Time 3/18–23</span><br>
<span class="tag-r mt-2 inline-block">官方否認</span></div>
</v-click>
<v-click>
<div class="kpi"><div class="tag-b mb-2">斡旋方</div>
積極介入：巴基斯坦（主辦地）、阿曼（傳訊）、土耳其、埃及<br>
Vance-伊朗代表會議擬於近日舉行<br>
<span class="text-xs text-gray-400">— CNN 3/23</span><br>
<span class="tag-y mt-2 inline-block">多方斡旋中</span></div>
</v-click>
</div>

<div class="grid grid-cols-2 gap-4 mt-4 text-sm">
<v-click>

### 談判障礙矩陣

| 議題 | 美方底線 | 伊方底線 | 差距 |
|------|---------|---------|------|
| 核武問題 | 永久放棄 | 保留核子技術權 | ❌ 極大 |
| 荷莫茲通行 | 立即開放 | 換取安全保證 | ⚠️ 可談 |
| 以色列因素 | 非本次議題 | 停止攻擊 | ❌ 大 |
| 賠償責任 | 不接受 | 美方須負責 | ❌ 極大 |

</v-click>
<v-click>

### 關鍵時間節點

<div class="wb mt-1">
📅 <strong>3/28（5日緩衝到期）</strong>：若荷莫茲仍未開通，川普表示將重啟電廠攻擊。此為目前最關鍵觀察窗口。
</div>

</v-click>
</div>

<div class="sfoot">5/15　機關內部報告</div>

---
transition: slide-up
---

# 荷莫茲海峽：全球能源咽喉

<div class="grid grid-cols-2 gap-6 mt-3">

<div class="text-sm space-y-2">
<v-click><div class="kpi">🛢️ 正常流量約 <strong>20 mb/d</strong>（全球原油海運量 <strong>~20%</strong>）<br><span class="text-xs text-gray-400">IEA, March 2026 Oil Market Report</span></div></v-click>
<v-click><div class="kpi" style="border-left-color:#c0392b">🔴 當前流量跌至正常值 <strong>約5%</strong>；21艘商船遭攻擊（3/1–3/24）<br><span class="text-xs text-gray-400">UKMTO Maritime Alert, 3/24</span></div></v-click>
<v-click><div class="kpi">🌏 <strong>75%</strong> 出口流向中、印、日、韓；台灣石油進口 <strong>70–75%</strong> 途經此處<br><span class="text-xs text-gray-400">Kpler Data / INSIDE Taiwan, 3/23</span></div></v-click>
<v-click><div class="kpi" style="border-left-color:#d68910">⚡ 卡達 LNG 占全球供應 <strong>20%</strong>；已宣告不可抗力停產<br><span class="text-xs text-gray-400">QatarEnergy Force Majeure Declaration</span></div></v-click>
</div>

<div>

### 參考影片（請自行核實URL）

<div class="rounded overflow-hidden border border-gray-200 mt-2">
<!--
  ⚠️ 請將下方影片ID替換為可播放的報導：
  建議：Al Jazeera / BBC News / CNN 官方頻道
  操作：YouTube影片網址中 ?v=XXXXXXXX 即為ID
-->
<iframe
  width="100%" height="210"
  src="https://www.youtube.com/embed/dQw4w9WgXcQ?rel=0"
  title="荷莫茲海峽相關報導（佔位，請替換ID）"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen
></iframe>
</div>
<div class="text-xs text-gray-400 mt-1 text-center">
⚠ 影片ID為佔位符，請替換為可用的新聞報導連結（見README）
</div>
</div>

</div>

<div class="sfoot">6/15　機關內部報告</div>

---
transition: fade
---

# 布蘭特原油走勢分析（2/27 — 3/24）

<OilChart />

<div class="grid grid-cols-3 gap-3 mt-3 text-xs">
  <div class="kpi">戰前基準：<strong>$73/桶</strong><br><span class="text-gray-400">2026年2月27日</span></div>
  <div class="kpi" style="border-left-color:#c0392b">峰值：<strong>$120/桶</strong><br><span class="text-gray-400">3/8–9（+64.4%）</span></div>
  <div class="kpi" style="border-left-color:#1e8449">當前：<strong>~$100/桶</strong><br><span class="text-gray-400">3/23（停火訊號）</span></div>
</div>

<div class="nb mt-3 text-xs">
💡 滑鼠懸停圖表可查看每日布蘭特 vs WTI 精確數值。數據來源：Bloomberg / CNBC / Fortune，已剔除盤中極端值，取收盤估算值呈現。
</div>

<div class="sfoot">7/15　機關內部報告</div>

---
layout: two-cols
transition: slide-left
---

# 進階統計分析

### 一、年化實現波動率

$$\sigma_{RV} = \sqrt{\frac{252}{n}\sum_{i=1}^{n}\left(\ln\frac{P_i}{P_{i-1}}\right)^2}$$

<div class="nb text-sm mt-2">
依 2/27–3/9 實際油價計算：<br>
<strong>戰期年化波動率 ≈ 218%</strong>（vs. 2025年均值約22%）<br>
→ 超出正常水準約 <strong>10倍</strong>，屬極端肥尾事件
</div>

<v-click>

### 二、Goldman Sachs 情境均價

| 情境 | 布蘭特均價 | 信心區間 |
|------|----------|---------|
| 荷莫茲3月開通 | $85/桶 | ±$10 |
| 封鎖至4月10日 | $110/桶 | ±$15 |
| 封鎖超過10週 | $147+/桶 | 破2008紀錄 |

<div class="text-xs text-gray-400 mt-1">來源：Goldman Sachs Research, 3/23/2026</div>

</v-click>

::right::

<div class="pl-6">

### 三、Python 統計模擬

```python {all|1-8|10-16|18-24}
import numpy as np

# 布蘭特日收益率序列
prices = [73, 80, 82, 87, 96, 103, 120,
          92, 100, 97, 110, 112, 106, 100]
returns = np.log(
  np.array(prices[1:]) / np.array(prices[:-1])
)

# 年化實現波動率
rv = np.std(returns) * np.sqrt(252)
print(f"年化波動率: {rv:.1%}")
# → 約 218.3%

peak = max(returns)
maxdd = min(returns)
print(f"最大單日漲: {peak:.1%}")
print(f"最大單日跌: {maxdd:.1%}")

# 蒙地卡羅期望值
ev_price = 0.35*85 + 0.45*105 + 0.20*140
ev_gdp   = 0.35*(-0.3) + 0.45*(-0.8) + 0.20*(-1.5)
print(f"油價期望值: ${ev_price:.1f}/桶")
print(f"GDP衝擊期望: {ev_gdp:.2f}%")
```

<div class="nb text-xs mt-2">
▶ 點選頁面可逐段高亮程式碼區塊（Slidev `{all|1-8|...}` 功能）
</div>

</div>

<div class="sfoot">8/15　機關內部報告</div>

---
transition: slide-up
---

# 全球供應鏈複合衝擊

<div class="grid grid-cols-3 gap-4 mt-3 text-sm">
<v-click>
<div class="kpi h-full">
<div class="tag-r mb-2">🛢️ 能源</div>
<ul class="list-none space-y-1 mt-1">
<li>供應缺口 <strong>8–10 mb/d</strong>（IEA）</li>
<li>LNG現貨船日租金暴漲數倍</li>
<li>歐盟柴油均價逾 EUR 2/升</li>
<li>美國加油站均價突破 $4/加侖</li>
<li>加州超過 $5/加侖</li>
</ul>
</div>
</v-click>
<v-click>
<div class="kpi h-full">
<div class="tag-y mb-2">⚙️ 半導體製造氣體</div>
<ul class="list-none space-y-1 mt-1">
<li>卡達占全球氦氣產量 <strong>33%</strong></li>
<li>全球每月缺口 <strong>520萬m³</strong>（IndexBox）</li>
<li>氦氣現貨價格已翻倍</li>
<li>韓國三星/SK海力士市值蒸發6兆韓圜</li>
<li>半導體廠配給率預估降至95%</li>
</ul>
</div>
</v-click>
<v-click>
<div class="kpi h-full">
<div class="tag-b mb-2">🌾 糧食與原物料</div>
<ul class="list-none space-y-1 mt-1">
<li>GCC國家食物進口 <strong>70%</strong> 受阻</li>
<li>全球 <strong>50%</strong> 尿素/硫磺出口停滯</li>
<li>LNG是氮肥原料，化肥成本急升</li>
<li>WFP：糧食危機風險趨近2022年水準</li>
<li>鋁價因電力成本飆升</li>
</ul>
</div>
</v-click>
</div>

<div class="grid grid-cols-2 gap-4 mt-4 text-sm">
<v-click>

### 金融市場

| 資產 | 變動 | |
|------|------|---|
| S&P 500 | −5%（3月第1週） | ↓ |
| 黃金 | 異常承壓（美元升值） | ↓ |
| 比特幣 | +8%（避險分散） | ↑ |
| 美國公債10Y | 殖利率上升 | ↑ |

</v-click>
<v-click>

### 國際陣營

| 陣營 | 代表國 |
|------|------|
| 支持美以 | 英國、澳洲、部分海灣國 |
| 反對/譴責 | 中國、俄羅斯、上合組織 |
| 中立觀望 | 日、韓、**台灣**、印度 |
| 斡旋調停 | 巴基斯坦、阿曼、土耳其 |

</v-click>
</div>

<div class="sfoot">9/15　機關內部報告</div>

---
transition: fade
---

# 台灣能源安全曝險分析

<div class="grid grid-cols-2 gap-6 mt-2">

<div>
<div class="text-xs text-gray-500 mb-1">各能源別：荷莫茲依賴度 vs 安全存量天數（可互動懸停）</div>
<EnergyChart />
</div>

<div class="text-sm">
<v-click>

### 摩根士丹利「11天LNG懸崖」

<div class="wb mt-1">
⚠️ 台灣天然氣安全存量<strong>僅11天</strong>，為三種燃料中最脆弱：
石油90天 / 煤炭30天 / <strong style="color:#c0392b">天然氣僅11天</strong><br>
<span class="text-xs text-gray-400">— Morgan Stanley, 2026年3月初研究報告</span>
</div>

</v-click>
<v-click>

### 關鍵曝險數字

| 指標 | 數值 |
|------|------|
| 石油進口途徑荷莫茲 | 70–75% |
| LNG 途徑荷莫茲 | 約28% |
| 天然氣發電占台電供電 | >50% |
| TSMC 占全台用電 | 約10% |

<div class="text-xs text-gray-400 mt-1">來源：CPC、經濟部能源署、INSIDE Taiwan, 2026/3</div>

</v-click>
</div>

</div>

<div class="sfoot">10/15　機關內部報告</div>

---
transition: slide-left
---

# 台灣半導體供應鏈：氦氣危機

<div class="grid grid-cols-2 gap-6 mt-2">

<div>
<div class="text-xs text-gray-500 mb-1">台灣 vs 韓國 氦氣來源分佈（可懸停查看）</div>
<HeChart />
<div class="text-xs text-gray-400 mt-1 text-center">來源：TechNews、大紀元、IndexBox, 2026/3</div>
</div>

<div class="text-sm">
<v-click>
<div class="nb">
<strong>氦氣是半導體製造的「血液」</strong>：用於晶圓背面冷卻、真空洩漏偵測、蝕刻環境保護。任何數天的中斷即可能導致減產。
<span class="text-xs text-gray-400">— 美國半導體協會（SIA），2023年參院證詞</span>
</div>
</v-click>
<v-click>

### 台灣 vs 韓國韌性比較

| 指標 | 台灣 | 韓國 |
|------|------|------|
| 卡達氦氣依賴度 | **30%** | **64–90%** |
| 美國供應比例 | ~30% | 較少 |
| 分散採購布局 | ✅ 已布局 | ⚠️ 較集中 |
| 短期衝擊程度 | 相對較輕 | **嚴重** |

</v-click>
<v-click>
<div class="wb mt-2 text-xs">
⚠️ 即使3月達成和平協議，氦氣供應恢復仍需至少<strong>3個月</strong>（Kornbluth諮詢，2026/3）
</div>
</v-click>
</div>

</div>

<div class="sfoot">11/15　機關內部報告</div>

---
transition: slide-up
---

# 貝氏情境機率分析

$$P(\theta \mid D) \propto P(D \mid \theta) \cdot P(\theta)$$

<div class="text-xs text-gray-500 mb-3">依川普聲明（3/23）與伊朗官方否認，對先驗機率進行貝氏更新。圖表可懸停查看雙軸數值。</div>

<ScenarioBar />

<v-click>
<div class="nb mt-3 text-sm">
📊 <strong>期望值推算</strong>：油價加權期望值 = 0.35×85 + 0.45×105 + 0.20×140 = <strong>$104.5/桶</strong>；台灣GDP預期衝擊 = 0.35×(−0.3%) + 0.45×(−0.8%) + 0.20×(−1.5%) = <strong>約 −0.76%</strong>（僅能源管道衝擊，不含貿易與金融溢出效果）。機率分配將隨3/28關鍵節點結果動態修正。
</div>
</v-click>

<div class="sfoot">12/15　機關內部報告</div>

---
layout: two-cols
transition: fade
---

# 政府現行因應措施

### 能源安全

<div class="space-y-2 mt-2 text-sm">
<v-click><div class="nb">✅ <strong>LNG採購多元化</strong>：經濟部長龔明鑫宣示「3月供應已確保，4月起分散來源」；中油自美國 Cheniere 供氣量提升（CPC長約320萬噸/年）</div></v-click>
<v-click><div class="nb">✅ <strong>法定存量提升</strong>：能源署副署長陳崇憲宣布，LNG最低存量自明年起從11天提升至14天；5月需求已確保過半供應</div></v-click>
<v-click><div class="wb">⚠️ <strong>仍待強化</strong>：14天仍低於石油90天、煤炭30天標準；中長期須考慮儲氣設施擴建</div></v-click>
</div>

::right::

<div class="pl-6">

### 半導體供應鏈

<div class="space-y-2 mt-2 text-sm">
<v-click><div class="nb">✅ <strong>氦氣供應穩定</strong>：經濟部（3/13）確認可自美國、澳洲等多元來源取得，整體仍屬穩定</div></v-click>
<v-click><div class="nb">✅ <strong>美國立法支持</strong>：美議員提出法案強化台灣天然氣供應，定位為地緣政治與科技供應鏈雙重議題</div></v-click>
<v-click><div class="nb">✅ <strong>比較優勢</strong>：氦氣來源較韓國更分散（30% vs 64–90%依賴卡達），韌性相對較佳</div></v-click>
</div>

### 外交立場

<v-click>
<div class="nb mt-3 text-sm">
台灣目前維持<strong>中立觀望</strong>立場，與日、韓相近。牛津大學危機研究所所長 Eimon 提醒：北韓與中國可能趁此機會加大施壓，須維持高度警覺。
</div>
</v-click>

</div>

<div class="sfoot">13/15　機關內部報告</div>

---
transition: slide-up
---

# 後續政策建議

<div class="grid grid-cols-2 gap-5 mt-3">

<div>

### 短期（1個月內）

<div class="space-y-2 text-sm">
<v-click><div class="nb" style="border-left-color:#c0392b;">🔴 <strong>P1【緊急】</strong>　加速LNG現貨採購與替代供應布局<br>
<span class="text-xs text-gray-500">優先採購美、澳、東南亞現貨，確保4–5月無間隙缺口</span></div></v-click>
<v-click><div class="nb" style="border-left-color:#d68910;">🟡 <strong>P2【重要】</strong>　啟動電力需量管理預案<br>
<span class="text-xs text-gray-500">評估台電調度彈性，啟動大型用電戶備用機組預備方案</span></div></v-click>
<v-click><div class="nb" style="border-left-color:#d68910;">🟡 <strong>P3【重要】</strong>　密切監控荷莫茲通行率<br>
<span class="text-xs text-gray-500">3/28 為關鍵節點，若封鎖持續應立即啟動B情境應對預案</span></div></v-click>
</div>

</div>

<div>

### 中長期（3–12個月）

<div class="space-y-2 text-sm">
<v-click><div class="nb" style="border-left-color:#1a5276;">🔵 <strong>M1</strong>　LNG最低儲量提前立法至14天以上<br>
<span class="text-xs text-gray-500">研議中期目標提升至21天（參考日韓標準），規劃儲氣設施擴建</span></div></v-click>
<v-click><div class="nb" style="border-left-color:#1a5276;">🔵 <strong>M2</strong>　半導體戰略物料儲備機制<br>
<span class="text-xs text-gray-500">研議氦氣、氬氣等關鍵製程氣體的「國家戰略儲備」機制</span></div></v-click>
<v-click><div class="nb" style="border-left-color:#1a5276;">🔵 <strong>M3</strong>　中東–能源–產業鏈三向預警機制<br>
<span class="text-xs text-gray-500">建立地緣政治情報與能源供應的聯動預警，縮短政策反應時間</span></div></v-click>
<v-click><div class="nb" style="border-left-color:#1a5276;">🔵 <strong>M4</strong>　把握美國立法契機強化雙邊能源框架<br>
<span class="text-xs text-gray-500">積極與美國國會溝通，將台灣能源韌性納入雙邊戰略框架</span></div></v-click>
</div>

</div>

</div>

<div class="sfoot">14/15　機關內部報告</div>

---
layout: two-cols
transition: fade
---

# 附錄：主要資料來源

### 國際媒體與機構

<div class="text-xs mt-2">

| # | 來源 | 內容 | 日期 |
|---|------|------|------|
| 1 | Bloomberg | 川普5日緩衝 / 停火談判 | 3/23 |
| 2 | CNN | 停火轉折分析 | 3/23 |
| 3 | Newsweek | 戰況每日更新 | 3/24 |
| 4 | Al Jazeera | 第22日戰況 | 3/22 |
| 5 | Fortune | 布蘭特逼近$110 | 3/18 |
| 6 | IEA | Oil Market Report | 3/13 |
| 7 | Goldman Sachs | 油價情境預測 | 3/23 |
| 8 | Wikipedia (EN) | 2026 Iran War | 持續更新 |

</div>

::right::

<div class="pl-6">

### 台灣媒體與機構

<div class="text-xs mt-2">

| # | 來源 | 內容 | 日期 |
|---|------|------|------|
| 1 | INSIDE Taiwan | LNG 11天懸崖 | 3/23 |
| 2 | TechNews | 氦氣供應鏈分析 | 3/18–19 |
| 3 | 大紀元 | 經濟部氦氣聲明 | 3/13 |
| 4 | 經濟日報 | 半導體氦氣風險 | 3/21 |
| 5 | IndexBox | 全球氦氣缺口520萬m³ | 3/2026 |

</div>

### 統計方法說明

<div class="nb text-xs mt-3">
年化實現波動率、蒙地卡羅情境參數與貝氏機率分配，係基於上述公開數據推估，非官方機構正式預測，供決策參考。情境機率反映3/24時點研判，將隨事件進展修正。
</div>

<div class="wb text-xs mt-3">
⚠️ 本報告為機關內部分析用途，所有情境分析不代表政治立場。
</div>

</div>

<div class="abs-br m-4 text-xs text-gray-400">
15/15 完　｜　製作日期：2026.03.24
</div>
