# 程序控制 / Process Control — NTUST

國立臺灣科技大學【化工系】程序控制 / 【先進科技專班】程序控制 課程教材：互動教學網頁（中英文）與講義。

Course materials for **Process Control** at NTUST — Department of Chemical Engineering / Advanced Technology Program. Interactive tutorials (EN/ZH) and lecture notes.

---

## 資料夾結構 / Repository Structure

| 資料夾 | 內容 | Content |
|--------|------|---------|
| [`00_math_toolbox`](00_math_toolbox/) | 工程數學工具箱（M1–M16） | Engineering Math Toolbox — 16 topics |
| [`01_ch1ch2`](01_ch1ch2/) | Chapter 1–2 程序控制基礎 | Process Control Fundamentals |

---

## 快速開啟 / Quick Access (GitHub Pages)

### 00 — 工程數學工具箱 / Math Toolbox

| 語言 | 連結 |
|------|------|
| English | [math_toolbox_interactive_EN.html](https://ylyang731223.github.io/process-control-ntustche/00_math_toolbox/math_toolbox_interactive_EN.html) |
| 中文 | [math_toolbox_互動教學.html](https://ylyang731223.github.io/process-control-ntustche/00_math_toolbox/math_toolbox_互動教學.html) |

### 01 — Chapter 1–2

| 語言 | 連結 |
|------|------|
| English | [ch1ch2_interactive_EN.html](https://ylyang731223.github.io/process-control-ntustche/01_ch1ch2/ch1ch2_interactive_EN.html) |
| 中文 | [ch1ch2_互動教學.html](https://ylyang731223.github.io/process-control-ntustche/01_ch1ch2/ch1ch2_互動教學.html) |

> 需先啟用 GitHub Pages（Settings → Pages → Source: `main` / `/ (root)`）

---

## 課程章節總覽 / Course Outline

### 00 — 工程數學工具箱 (M1–M16)

貫穿全課程的 16 個數學先備知識，每個主題含公式、直覺理解、逐步推導、練習題與課程連結。

| # | 主題 | Topic | 對應章節 |
|---|------|-------|----------|
| M1 | 分部積分 | Integration by Parts | Ch1-2, Ch6 |
| M2 | 瑕積分 | Improper Integrals | Ch1-2, Ch3–Ch8 |
| M3 | 羅必達法則 | L'Hôpital's Rule | Ch1-2, Ch3, Ch6 |
| M4 | 歐拉公式 | Euler's Formula | Ch1-2, Ch7, Ch15–16 |
| M5 | 複數基礎 | Complex Number Basics | Ch1-2, Ch3, Ch7–8, Ch13, Ch15–17 |
| M6 | 雙曲函數 | Hyperbolic Functions | Ch1-2, Ch13 |
| M7 | 部分分式分解技巧 | Partial Fraction Techniques | Ch1-2, Ch3, Ch6, Ch8, Ch12 |
| M8 | 積分因子法推導 | Integrating Factor Derivation | Ch1-2, Ch4 |
| M9 | Taylor 展開與線性化 | Taylor Series & Linearization | Ch5, Ch7, Ch12 |
| M10 | 對數與分貝 | Logarithms & Decibels | Ch4, Ch15–16 |
| M11 | 終值定理與初值定理 | Final & Initial Value Theorems | Ch3, Ch8, Ch11–12 |
| M12 | 多項式長除法 | Polynomial Long Division | Ch3, Ch6 |
| M13 | 特徵方程式、極點與零點 | Characteristic Eq., Poles & Zeros | Ch3, Ch6–8, Ch11–13, Ch17 |
| M14 | Routh-Hurwitz 穩定性判據 | Routh-Hurwitz Stability Criterion | Ch11–13 |
| M15 | 頻率響應 s=jω | Frequency Response | Ch4, Ch7, Ch15–16 |
| M16 | Padé 近似 | Padé Approximation | Ch7, Ch12 |

### 01 — Chapter 1–2 程序控制基礎

| Unit | 主題 | Topic |
|------|------|-------|
| 1 | 為什麼需要程序控制？ | Why Do We Need Process Control? |
| 2 | 閉迴路控制系統方塊圖 | Control System Block Diagram |
| 3 | 化學混合槽與物料平衡 | Mixing Tank & Material Balance |
| 4 | 一階系統求解與 Step Response | First-Order System Solution & Step Response |
| 5 | 能量平衡與標準一階形式 | Energy Balance & Standard First-Order Form |
| 6 | Laplace 轉換基礎 | Laplace Transform Fundamentals |
| 6→7 | 微分的 Laplace 轉換（補充） | Transforms of Derivatives (Supplement) |
| 7 | 轉移函數 | Transfer Function |
| 8 | 部分分式與根的型態 | Partial Fractions & Root Types |

---

## 互動功能 / Interactive Features

- **逐步推導展開** — 點擊逐步顯示完整數學推導過程
- **練習題** — 每個主題附簡單例題，可展開步驟與答案
- **互動圖表** — 拖曳滑桿即時改變參數，觀察系統響應變化
- **可點擊方塊圖** — 點選控制系統方塊，顯示對應說明
- **隨堂測驗** — 每個 Unit 附選擇題，即時回饋
- **側邊欄導航** — 快速跳轉至任一主題
- **中英雙語** — 每份教材皆提供英文與中文版本

---

## 使用方式 / How to Use

### 方法一：GitHub Pages（推薦）

啟用 GitHub Pages 後，點擊上方「快速開啟」連結即可在瀏覽器中直接使用。

### 方法二：下載後本機開啟

1. 點擊綠色 **Code** 按鈕 → **Download ZIP**
2. 解壓縮後，用瀏覽器開啟 `.html` 檔案

### 方法三：git clone

```bash
git clone https://github.com/ylyang731223/process-control-ntustche.git
cd process-control-ntustche
# 開啟互動教學網頁
start 01_ch1ch2/ch1ch2_interactive_EN.html   # Windows
```

---

## 技術資訊 / Technical Notes

- 數學公式渲染：KaTeX（CDN 載入，需網路連線）
- 圖表：SVG + Canvas
- 純前端，無需後端伺服器
