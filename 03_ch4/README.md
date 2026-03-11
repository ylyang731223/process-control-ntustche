# Ch4 — 一階系統的動態響應 / First-Order System Dynamic Response

本資料夾包含程序控制課程 Chapter 4 的互動教學網頁與講義。

This folder contains interactive tutorials and lecture notes for **Process Control** Chapter 4.

---

## 檔案說明 / Files

| 檔案 | 說明 |
|------|------|
| `ch4_interactive_EN.html` | 英文互動式教學網頁 (English interactive tutorial) |
| `ch4_互動教學.html` | 中文互動式教學網頁 (Chinese interactive tutorial) |
| `ch4_lecture_notes.docx` | 中英雙語講義 Word 版本 (Bilingual lecture notes, Word) |

---

## 課程架構 / Course Structure (5 Units)

| Unit | 主題 | Topic |
|------|------|-------|
| 1 | 溫度計 — 一階物理系統 | Thermometer — A First-Order Physical System |
| 2 | 一階系統的階躍響應 | Step Response of First-Order Systems |
| 3 | 脈衝響應與斜坡響應 | Impulse & Ramp Response |
| 4 | 正弦響應與頻率分析 | Sinusoidal Response & Frequency Analysis |
| 5 | 範例 4.3 與總結 | Example 4.3 & Summary |

---

## 互動功能 / Interactive Features

- **溫度計 SVG 示意圖** — Unit 1 溫度計物理系統示意圖（液體、水銀、玻璃壁），對應能量平衡推導
- **逐步推導展開** — 溫度計能量平衡 → 標準一階形式 → 轉移函數 $G(s) = K_p/(\tau s+1)$；階躍 / 脈衝 / 斜坡 / 正弦響應完整推導
- **為什麼要學三種標準輸入** — 框架說明 Step / Ramp / Sinusoidal 各測試什麼動態特性
- **初始斜率與切線幾何意義** — 4 步推導 $dY/dt|_{t=0} = K_pA/\tau$，切線在 $t=\tau$ 碰到最終值
- **安定時間表格** — $1\tau$ 至 $5\tau$ 的誤差帶與百分比
- **常見誤解** — 5 項常見迷思與正確理解對照表
- **物理解釋與核心問題** — 每種響應的核心問題（「系統多快到新穩態？」「能否持續追上？」「如何處理振盪？」）
- **圖形判讀指南** — 教學生如何看懂 Step / Ramp / Sinusoidal 互動圖表
- **常見考點** — 每種響應的結構化考試重點整理
- **互動圖表（Canvas）**：
  - **Step Response** — 拖曳 $\tau$、$K_p$、$A$ 滑桿，即時觀察輸入（綠色虛線）、輸出（藍色實線）、最終值、初始切線（紅色點線）、$3\tau$ / $5\tau$ 里程碑標記
  - **Ramp Response (Figure 4–16)** — 拖曳 $\tau$、$K_p$、$b$ 滑桿，顯示時間滯後 $\tau$ 和偏移 $K_pb\tau$
  - **Sinusoidal Response (Figure 4–17)** — 拖曳 $\tau$、$K_p$、$A$、$\omega$ 滑桿，顯示暫態包絡線、振幅比 AR、相位滯後 $\phi$
  - **Example 4.3 (Figure 4–18)** — 溫度計正弦輸入響應：液體溫度 vs. 溫度計讀數，週期 0.314 min
- **波德圖概念簡介** — 振幅圖 / 相位圖、轉角頻率 $\omega_c = 1/\tau$、低通濾波器特性
- **統整比較表** — 增加 $\tau$ 對三種輸入的影響：更慢、追隨更差、更傾向濾除
- **隨堂測驗** — 每個 Unit 附 2 題選擇題，即時回饋答案
- **進度追蹤** — 側邊欄顯示完成進度

---

## 核心內容 / Key Content

### Unit 1 — 溫度計模型 / Thermometer Model

從溫度計的能量平衡推導出標準一階轉移函數：

$$G(s) = \frac{K_p}{\tau s + 1}$$

其中 $\tau = C_m/(hA)$（熱容量 / 熱傳係數 × 面積），$K_p = 1$（溫度計最終讀取真實溫度）。

### Unit 2 — 階躍響應 / Step Response

$$y(t) = K_pA\left(1 - e^{-t/\tau}\right)$$

| 時間 | 達到最終值 % | 剩餘誤差 |
|------|------------|----------|
| $1\tau$ | 63.2% | 36.8% |
| $3\tau$ | 95.0% | 5.0% |
| $4\tau$ | 98.2% | 1.8%（2% 安定） |
| $5\tau$ | 99.3% | 0.7%（1% 安定） |

**幾何意義：** $t=0$ 處切線（斜率 $K_pA/\tau$）在 $t=\tau$ 時恰好達到最終值 $K_pA$。

### Unit 3 — 脈衝與斜坡響應 / Impulse & Ramp Response

| 輸入 | 響應 |
|------|------|
| 脈衝 $A\delta(t)$ | $y(t) = (K_pA/\tau)\,e^{-t/\tau}$ |
| 斜坡 $bt$ | $y(t) = K_pb\left(t - \tau + \tau\,e^{-t/\tau}\right)$ |

**斜坡響應特徵：** 永久時間滯後 $\tau$，永久偏移 $K_pb\tau$。$K_p=1$ 時輸出為輸入平移 $\tau$。

### Unit 4 — 正弦響應與頻率分析 / Sinusoidal Response & Frequency Analysis

$$y_{ss}(t) = \frac{K_pA}{\sqrt{1+\omega^2\tau^2}}\sin(\omega t + \phi), \quad \phi = -\arctan(\omega\tau)$$

| $\omega\tau$ | $AR/K_p$ | 相位滯後 |
|------|------|------|
| 0.1 | 0.995 | $-5.7°$ |
| 1.0 | 0.707 | $-45°$ |
| 10 | 0.0995 | $-84.3°$ |

**低通濾波器：** 低頻通過，高頻衰減。轉角頻率 $\omega_c = 1/\tau$。

### Unit 5 — 統整比較 / Comparative Summary

| 輸入類型 | 核心問題 | 增加 $\tau$ 的後果 |
|----------|---------|------------------|
| 階梯 Step | 多快到新穩態？ | 更慢（系統更遲鈍） |
| 斜坡 Ramp | 能否持續追上？ | 落後更明顯（追隨變差） |
| 正弦 Sinusoidal | 如何處理振盪？ | 振幅更小、相位滯後更大 |

---

## 例題總覽 / Worked Examples

| 例題 | Unit | 內容 | 結果 |
|------|------|------|------|
| Thermometer derivation | 1 | 溫度計能量平衡 → 轉移函數 | $G(s) = 1/(\tau s + 1)$ |
| Step response | 2 | 一階系統階躍響應推導 | $y(t) = K_pA(1-e^{-t/\tau})$ |
| Impulse response | 3 | 脈衝響應推導 | $y(t) = (K_pA/\tau)e^{-t/\tau}$ |
| Ramp response | 3 | 斜坡響應推導 | $y(t) = K_pb(t-\tau+\tau e^{-t/\tau})$ |
| Sinusoidal response | 4 | 正弦響應推導 | $AR = K_p/\sqrt{1+\omega^2\tau^2}$, $\phi=-\arctan(\omega\tau)$ |
| Example 4.3 (step) | 5 | 溫度計 $\tau=0.1$ min，階躍響應 | $T_m(0.1) = 34.48°C$ |
| Example 4.3 (sine) | 5 | 溫度計正弦輸入，週期 0.314 min | AR = 0.447，振幅 0.894°C，滯後 0.056 min |

---

## 使用方式 / How to Use

### 本機開啟 / Local

1. 用瀏覽器開啟 `ch4_interactive_EN.html`（英文）或 `ch4_互動教學.html`（中文）
2. 點擊左側 sidebar 選擇 Unit
3. 點擊「Next Step →」逐步展開推導
4. 拖曳 Unit 2–5 的滑桿觀察響應曲線變化
5. 完成每個 Unit 的隨堂測驗

### 在 GitHub 上開啟 / Open from GitHub

**方法一：GitHub Pages（推薦）**

若 repository 已啟用 GitHub Pages（Settings → Pages → Source: `main` / `/ (root)`），可直接用以下網址開啟：

| 語言 | 連結 |
|------|------|
| English | [ch4_interactive_EN.html](https://ylyang731223.github.io/process-control-ntustche/03_ch4/ch4_interactive_EN.html) |
| 中文 | [ch4_互動教學.html](https://ylyang731223.github.io/process-control-ntustche/03_ch4/ch4_互動教學.html) |

**方法二：下載後本機開啟**

1. 前往 [repository 首頁](https://github.com/ylyang731223/process-control-ntustche)
2. 點擊綠色 **Code** 按鈕 → **Download ZIP**
3. 解壓縮後，直接用瀏覽器開啟 `.html` 檔案

**方法三：使用 `git clone`**

```bash
git clone https://github.com/ylyang731223/process-control-ntustche.git
cd process-control-ntustche/03_ch4
# 用瀏覽器開啟
start ch4_interactive_EN.html   # Windows
open ch4_interactive_EN.html    # macOS
xdg-open ch4_interactive_EN.html  # Linux
```

---

## 技術資訊 / Technical Notes

- 數學公式渲染：KaTeX（CDN 載入，需網路連線）
- 圖表：SVG（溫度計示意圖）+ Canvas（Step / Ramp / Sinusoidal / Example 4.3 互動響應曲線）
- 互動滑桿：即時調整 $\tau$、$K_p$、$A$、$\omega$、$b$ 等參數
- 深色模式：支援系統偏好設定自動切換
- 純前端，無需後端伺服器
