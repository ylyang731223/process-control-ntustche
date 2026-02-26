# Ch1 & Ch2 — 程序控制基礎 / Process Control Fundamentals

本資料夾包含程序控制課程 Chapter 1–2 的互動教學網頁與講義。

This folder contains interactive tutorials and lecture notes for **Process Control** Chapters 1–2.

---

## 檔案說明 / Files

| 檔案 | 說明 |
|------|------|
| `ch1ch2_interactive_EN.html` | 英文互動式教學網頁 (English interactive tutorial) |
| `ch1ch2_互動教學.html` | 中文互動式教學網頁 (Chinese interactive tutorial) |
| `ch1ch2_lecture_notes.docx` | 中英雙語講義 (Bilingual lecture notes) |
| `ch1ch2_lecture_notes.pdf` | 講義 PDF 版本 |

---

## 課程架構 / Course Structure (8 Units)

### Chapter 1 — 為什麼需要程序控制 / Why Process Control

| Unit | 主題 | Topic |
|------|------|-------|
| 1 | 為什麼需要程序控制？ | Why Do We Need Process Control? |
| 2 | 閉迴路控制系統方塊圖 | Control System Block Diagram |

### Chapter 2 — 一階系統建模與求解 / First-Order System Modeling & Solution

| Unit | 主題 | Topic |
|------|------|-------|
| 3 | 化學混合槽與物料平衡 | Mixing Tank & Material Balance |
| 4 | 一階系統求解與 Step Response | First-Order System Solution & Step Response |
| 5 | 能量平衡與標準一階形式 | Energy Balance & Standard First-Order Form |
| 6 | Laplace 轉換基礎 | Laplace Transform Fundamentals |
| 6→7 | 微分的 Laplace 轉換（補充） | Transforms of Derivatives (Supplement) |
| 7 | 轉移函數 | Transfer Function |
| 8 | 部分分式與根的型態 | Partial Fractions & Root Types |

---

## 互動功能 / Interactive Features

- **逐步推導展開** — 物料平衡、能量平衡、積分因子法求解、Laplace 轉換推導（含 Table 2.1 全部 12 組完整推導）
- **微分轉換可點擊推導** — Transforms of Derivatives 表格（一階、二階、n 階），點擊列即展開完整推導（分部積分、遞推、數學歸納法）
- **互動圖表** — 拖曳滑桿即時改變 τ、Kp、A，觀察 Step Response 曲線變化（Canvas）
- **可點擊方塊圖** — 點選 R(s)、Gc(s)、Gp(s)、D(s) 等方塊，顯示對應說明
- **τ 與 Kp 物理意義 + 生活案例** — 浴缸 vs. 咖啡杯（τ）、稀釋果汁 / 調漆（Kp）等直覺比喻
- **加熱槽示意圖** — Unit 5 能量平衡示意圖（SVG / PNG），對照 Unit 3 混合槽
- **分頁式範例** — Unit 8 提供 5 種根型態的部分分式展開範例（相異實根、重根、共軛複數根、正實根、純虛根）
- **隨堂測驗** — 每個 Unit 附 1–3 題選擇題，即時回饋答案
- **進度追蹤** — 側邊欄顯示完成進度

---

## 核心內容 / Key Content

### 重要定義

| 符號 | 定義 |
|------|------|
| τ = V/v | 時間常數 = 滯留時間 (time constant = residence time) |
| Kp = v₃/v | 穩態增益 (steady-state gain) |
| Y(t) = Kp·A·(1 − e⁻ᵗ/τ) | 一階系統 Step Response |
| G(s) = Kp / (τs + 1) | 一階系統轉移函數 |

### τ 與 Kp 的物理意義 / Physical Meaning

- **τ（時間常數）**：系統達到 63.2% 穩態值所需時間；τ 越大，響應越慢。生活案例：浴缸 vs. 咖啡杯、尖峰時段高速公路。
- **Kp（穩態增益）**：輸入改變 1 單位時，輸出最終改變多少。生活案例：稀釋果汁、調和油漆顏色。

### Table 2.1 — Laplace Transform Pairs

包含 12 組 Laplace 轉換對及其完整推導：unit step、ramp、exponential decay、power、sine、cosine、hyperbolic sine/cosine、damped sine/cosine 等。

### Transforms of Derivatives — 微分的 Laplace 轉換

| 階數 | 公式 |
|------|------|
| 一階 | L{df/dt} = sF(s) − f(0) |
| 二階 | L{d²f/dt²} = s²F(s) − sf(0) − f'(0) |
| n 階 | L{dⁿf/dtⁿ} = sⁿF(s) − sⁿ⁻¹f(0) − ... − f⁽ⁿ⁻¹⁾(0) |

零初始條件下：微分直接變成乘以 s → 這正是轉移函數能成立的原因。

### 為什麼要學轉移函數 / Why Learn Transfer Functions

- 微分方程 → 代數：ODE 在 s 域變成代數方程
- 串接系統 = 相乘：G(s) = G₁(s)·G₂(s)
- 穩定性一目了然：極點實部為負 → 穩定
- 控制器設計的基礎：PID、根軌跡、Bode 圖皆建立於此

### 物料平衡 vs. 能量平衡對照表

以混合槽（物料）與加熱槽（能量）為例，對照兩種平衡的標準一階形式推導。能量平衡 Kp = 1（輸入輸出係數相同）。

---

## 使用方式 / How to Use

### 本機開啟 / Local

1. 用瀏覽器開啟 `ch1ch2_interactive_EN.html`（英文）或 `ch1ch2_互動教學.html`（中文）
2. 點擊左側 sidebar 選擇 Unit
3. 點擊「Next Step →」逐步展開推導
4. 拖曳 Unit 4 的滑桿觀察響應曲線
5. 完成每個 Unit 的隨堂測驗

### 在 GitHub 上開啟 / Open from GitHub

GitHub 無法直接在網頁內渲染 `.html` 檔案。以下提供三種方式：

**方法一：GitHub Pages（推薦）**

若 repository 已啟用 GitHub Pages（Settings → Pages → Source: `main` / `/ (root)`），可直接用以下網址開啟：

| 語言 | 連結 |
|------|------|
| English | [ch1ch2_interactive_EN.html](https://ylyang731223.github.io/process-control-ntustche/ch1ch2/ch1ch2_interactive_EN.html) |
| 中文 | [ch1ch2_互動教學.html](https://ylyang731223.github.io/process-control-ntustche/ch1ch2/ch1ch2_互動教學.html) |

**方法二：下載後本機開啟**

1. 前往 [repository 首頁](https://github.com/ylyang731223/process-control-ntustche)
2. 點擊綠色 **Code** 按鈕 → **Download ZIP**
3. 解壓縮後，直接用瀏覽器開啟 `.html` 檔案

**方法三：使用 `git clone`**

```bash
git clone https://github.com/ylyang731223/process-control-ntustche.git
cd process-control-ntustche/ch1ch2
# 用瀏覽器開啟
start ch1ch2_interactive_EN.html   # Windows
open ch1ch2_interactive_EN.html    # macOS
xdg-open ch1ch2_interactive_EN.html  # Linux
```

> `.docx` 可在 GitHub 頁面直接預覽；`.pdf` 可在線上檢視或下載。

---

## 技術資訊 / Technical Notes

- 數學公式渲染：KaTeX（CDN 載入，需網路連線）
- 圖表：SVG（方塊圖、混合槽示意圖、加熱槽示意圖）+ Canvas（互動響應曲線）
- 可點擊表格：Table 2.1（12 組）+ Transforms of Derivatives（3 組），點擊列展開推導
- 純前端，無需後端伺服器
- 講義字體：英文 Times New Roman / 中文標楷體

