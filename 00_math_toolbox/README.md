# 工程數學工具箱 / Engineering Math Toolbox (M1–M16)

本資料夾包含程序控制課程的「工程數學工具箱」互動教學網頁與講義，涵蓋 16 個核心數學主題。

This folder contains the **Engineering Math Toolbox** — interactive tutorials and bilingual lecture notes covering 16 essential math topics used throughout the Process Control course.

---

## 檔案說明 / Files

| 檔案 | 說明 |
|------|------|
| `math_toolbox_interactive_EN.html` | 英文互動式教學網頁 (English interactive tutorial) |
| `math_toolbox_互動教學.html` | 中文互動式教學網頁 (Chinese interactive tutorial) |
| `math_toolbox_lecture_notes.pdf` | 講義 PDF 版本 |

---

## 16 主題總覽 / 16 Topics Overview

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

---

## 每個主題包含 / Each Topic Includes

- **公式/定義** — 核心數學公式與定義
- **直覺理解** — 白話解釋為什麼需要這個工具
- **推導步驟** — 可展開的逐步推導（互動網頁）
- **練習題** — 1 題簡單例題，附步驟解答
- **課程連結** — 說明此工具在哪些章節被使用

---

## 互動功能 / Interactive Features

- **逐步展開推導** — 點擊「Show Steps →」/「展開步驟 →」逐步顯示推導過程
- **練習題互動** — 點擊「Try Example →」/「展開範例 →」展開例題步驟與答案
- **數學公式渲染** — KaTeX 即時渲染 LaTeX 數學式
- **側邊欄導航** — 快速跳轉至 M1–M16 任一主題
- **隨開即用** — 純前端，無需伺服器

---

## 使用方式 / How to Use

### 本機開啟 / Local

1. 用瀏覽器開啟 `math_toolbox_interactive_EN.html`（英文）或 `math_toolbox_互動教學.html`（中文）
2. 點擊左側 sidebar 選擇主題（M1–M16）
3. 點擊「Show Steps →」展開推導步驟
4. 點擊「Try Example →」練習例題

### 在 GitHub 上開啟 / Open from GitHub

**方法一：GitHub Pages（推薦）**

若 repository 已啟用 GitHub Pages，可直接用以下網址開啟：

| 語言 | 連結 |
|------|------|
| English | [math_toolbox_interactive_EN.html](https://ylyang731223.github.io/process-control-ntustche/00_math_toolbox/math_toolbox_interactive_EN.html) |
| 中文 | [math_toolbox_互動教學.html](https://ylyang731223.github.io/process-control-ntustche/00_math_toolbox/math_toolbox_互動教學.html) |

**方法二：下載後本機開啟**

1. 前往 [repository 首頁](https://github.com/ylyang731223/process-control-ntustche)
2. 點擊綠色 **Code** 按鈕 → **Download ZIP**
3. 解壓縮後，用瀏覽器開啟 `.html` 檔案

---

## 技術資訊 / Technical Notes

- 數學公式渲染：KaTeX（CDN 載入，需網路連線）
- 純前端，無需後端伺服器

