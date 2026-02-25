# Ch1 & Ch2 — 程序控制基礎 / Process Control Fundamentals

本資料夾包含程序控制課程 Chapter 1–2 的互動教學網頁與講義。

This folder contains interactive tutorials and lecture notes for **Process Control** Chapters 1–2.

---

## 檔案說明 / Files

| 檔案 | 說明 |
|------|------|
| `ch1ch2_interactive_EN.html` | 英文互動式教學網頁 (English interactive tutorial) |
| `ch1ch2_互動教學.html`（上層目錄） | 中文互動式教學網頁 (Chinese interactive tutorial) |
| `ch1ch2_lecture_notes.docx` | 中英雙語講義 (Bilingual lecture notes) |
| `ch1ch2_lecture_notes.pdf` | 講義 PDF 版本 |

> 直接用瀏覽器開啟 `.html` 檔案即可使用，不需要伺服器或網路連線。

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
| 7 | 轉移函數 | Transfer Function |
| 8 | 部分分式與根的型態 | Partial Fractions & Root Types |

---

## 互動功能 / Interactive Features

- **逐步推導展開** — 物料平衡、能量平衡、積分因子法求解、Laplace 轉換推導（含 Table 2.1 全部 12 組完整推導）
- **互動圖表** — 拖曳滑桿即時改變 τ、Kp、A，觀察 Step Response 曲線變化（Canvas）
- **可點擊方塊圖** — 點選 R(s)、Gc(s)、Gp(s)、D(s) 等方塊，顯示對應說明
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
| Y(t) = Kp·A·(1 − e^(−t/τ)) | 一階系統 Step Response |
| G(s) = Kp / (τs + 1) | 一階系統轉移函數 |

### Table 2.1 — Laplace Transform Pairs

包含 12 組 Laplace 轉換對及其完整推導：unit step、ramp、exponential decay、power、sine、cosine、hyperbolic sine/cosine、damped sine/cosine 等。

### 物料平衡 vs. 能量平衡對照表

以混合槽（物料）與加熱槽（能量）為例，對照兩種平衡的標準一階形式推導。

---

## 使用方式 / How to Use

1. 用瀏覽器開啟 `ch1ch2_interactive_EN.html`（英文）或 `ch1ch2_互動教學.html`（中文）
2. 點擊左側 sidebar 選擇 Unit
3. 點擊「Next Step →」逐步展開推導
4. 拖曳 Unit 4 的滑桿觀察響應曲線
5. 完成每個 Unit 的隨堂測驗

---

## 技術資訊 / Technical Notes

- 數學公式渲染：KaTeX
- 圖表：SVG（方塊圖、混合槽示意圖）+ Canvas（互動響應曲線）
- 純前端，無需後端伺服器
- 講義字體：英文 Times New Roman / 中文標楷體
