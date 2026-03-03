# Ch3 — 拉普拉斯轉換進階應用 / Advanced Laplace Transform Applications

本資料夾包含程序控制課程 Chapter 3 的互動教學網頁與講義。

This folder contains interactive tutorials and lecture notes for **Process Control** Chapter 3.

---

## 檔案說明 / Files

| 檔案 | 說明 |
|------|------|
| `ch3_interactive_EN.html` | 英文互動式教學網頁 (English interactive tutorial) |
| `ch3_互動教學.html` | 中文互動式教學網頁 (Chinese interactive tutorial) |
| `ch3_lecture_notes.docx` | 中英雙語講義 Word 版本 (Bilingual lecture notes, Word) |
| `ch3_lecture_notes.pdf` | 講義 PDF 版本 (Lecture notes, PDF) |

---

## 課程架構 / Course Structure (4 Units)

| Unit | 主題 | Topic |
|------|------|-------|
| 1 | 部分分式回顧與六種根 | Partial Fraction Review & Six Root Types |
| 2 | 複數根與 s 軸位移（Example 3.4） | Complex Roots & s-axis Shifting (Example 3.4) |
| 3 | 終值定理與初值定理 | Final & Initial Value Theorems |
| 4 | 自訂輸入函數建構（Example 3A.8） | Custom Input Construction (Example 3A.8) |

---

## 互動功能 / Interactive Features

- **六種根翻轉卡片** — 點擊卡片翻轉，顯示每種根的部分分式形式與時域表達式（相異實根、重根、共軛複數根、重複複數根、純虛根、零根）
- **Figure 3-1 s 平面根位置圖** — 顯示六種根在複數 $s$ 平面上的位置，附詳細表格說明每種根的位置、行為與穩定性
- **逐步推導展開** — 部分分式展開通用步驟、Example 3.4 完整求解、FVT/IVT 證明草稿、自訂輸入函數建構
- **互動圖表** — Example 3.4 時域響應曲線（Canvas），可視化 $x(t) = 1 - e^{-t}(\cos t + \sin t)$
- **SVG 示意圖** — 脈衝輸入、三角脈衝、階梯輸入等自訂輸入函數圖形
- **振幅-相位替代表示** — 展示 $e^{-at}(C_1\cos bt + C_2\sin bt)$ 的等效 $Re^{-at}\sin(bt+\phi)$ 形式
- **FVT / IVT 完整範例** — 包含 Example 3.4 驗證、一階系統 Step Response、Ramp Input 等多個應用範例
- **適用條件與摘要卡片** — 何時可用 FVT / IVT、何時不可用的判斷條件與整理
- **隨堂測驗** — 每個 Unit 附 2 題選擇題，即時回饋答案
- **進度追蹤** — 側邊欄顯示完成進度

---

## 核心內容 / Key Content

### Unit 1 — 部分分式回顧 / Partial Fraction Review

**六種根型態：**

| # | 根型態 | Root Type | 時域行為 |
|---|--------|-----------|----------|
| ① | 相異實根 | Distinct Real | $A_i e^{-a_i t}$ — 指數衰減 |
| ② | 重根 | Repeated Real | $(A_1 + A_2 t + \cdots)e^{-at}$ — 多項式 × 指數 |
| ③ | 共軛複數根 | Complex Conjugate | $e^{-at}(C_1\cos bt + C_2\sin bt)$ — 衰減振盪 |
| ④ | 重複複數根 | Repeated Complex | $t^k e^{-at}\sin(bt+\phi)$ — 高階衰減振盪 |
| ⑤ | 純虛根 | Pure Imaginary | $C_1\cos\omega t + C_2\sin\omega t$ — 持續振盪 |
| ⑥ | 零根 | Zero Root | $A \cdot u(t)$ — 常數（階梯函數） |

**穩定性法則 / Stability Rule from the s-Plane：**
- 左半平面 (Re < 0) → 穩定（衰減）
- 虛軸上 (Re = 0) → 邊際穩定（持續振盪 / 常數）
- 右半平面 (Re > 0) → 不穩定（發散）

### Unit 2 — Example 3.4 複數根求解

$$X(s) = \frac{2}{s(s^2+2s+2)} \quad \Rightarrow \quad x(t) = 1 - e^{-t}(\cos t + \sin t)$$

- 配方法：$(s+1)^2 + 1$ → 使用 s 軸位移定理
- Cover-up 求 $A$，係數比較求 $B, C$
- 互動圖表顯示時域響應曲線

### Unit 3 — 終值定理與初值定理 / Final & Initial Value Theorems

| 定理 | 公式 | 條件 |
|------|------|------|
| 終值定理 FVT | $\lim_{t\to\infty}f(t) = \lim_{s\to 0}sF(s)$ | $sF(s)$ 所有極點在左半平面 |
| 初值定理 IVT | $\lim_{t\to 0^+}f(t) = \lim_{s\to\infty}sF(s)$ | $F(s)$ 為嚴格真分式 |

### Unit 4 — 自訂輸入函數建構 / Custom Input Construction

以標準訊號（階梯、斜坡）搭配延遲與疊加原理，建構任意分段輸入函數：
- 矩形脈衝 Rectangular Pulse：$f(t) = h\,u(t) - h\,u(t-T)$
- 三角脈衝 Triangular Pulse：斜坡疊加
- 階梯輸入 Staircase：多重延遲階梯疊加

---

## 例題總覽 / Worked Examples

| 例題 | Unit | 內容 | 結果 |
|------|------|------|------|
| Example 3.4 | 2 | 複數根 $s=0, -1\pm i$ 部分分式展開 | $x(t) = 1 - e^{-t}(\cos t + \sin t)$ |
| FVT on Ex 3.4 | 3 | 驗證終值定理：$\lim sF(s)$ vs. $x(\infty)$ | 兩者皆 = 1 |
| IVT on Ex 3.4 | 3 | 驗證初值定理：$\lim sF(s)$ vs. $x(0^+)$ | 兩者皆 = 0 |
| First-Order FVT | 3 | 一階系統 Step Response 終值驗證 | $K_p A$ |
| Ramp Input IVT | 3 | Ramp 輸入初值驗證 | $f(0^+) = 0$ |
| Example 3A.8 | 4 | 矩形脈衝建構 | $F(s) = \frac{h}{s}(1-e^{-Ts})$ |
| Triangular Pulse | 4 | 三角脈衝建構 | 三段斜坡疊加 |
| Staircase Input | 4 | 階梯輸入建構 | 多重延遲階梯疊加 |

---

## 使用方式 / How to Use

### 本機開啟 / Local

1. 用瀏覽器開啟 `ch3_interactive_EN.html`（英文）或 `ch3_互動教學.html`（中文）
2. 點擊左側 sidebar 選擇 Unit
3. 點擊翻轉卡片查看六種根的詳細說明
4. 逐步展開 Example 3.4 的完整推導
5. 完成每個 Unit 的隨堂測驗

### 在 GitHub 上開啟 / Open from GitHub

**方法一：GitHub Pages（推薦）**

若 repository 已啟用 GitHub Pages（Settings → Pages → Source: `main` / `/ (root)`），可直接用以下網址開啟：

| 語言 | 連結 |
|------|------|
| English | [ch3_interactive_EN.html](https://ylyang731223.github.io/process-control-ntustche/02_ch3/ch3_interactive_EN.html) |
| 中文 | [ch3_互動教學.html](https://ylyang731223.github.io/process-control-ntustche/02_ch3/ch3_互動教學.html) |

**方法二：下載後本機開啟**

1. 前往 [repository 首頁](https://github.com/ylyang731223/process-control-ntustche)
2. 點擊綠色 **Code** 按鈕 → **Download ZIP**
3. 解壓縮後，直接用瀏覽器開啟 `.html` 檔案

**方法三：使用 `git clone`**

```bash
git clone https://github.com/ylyang731223/process-control-ntustche.git
cd process-control-ntustche/02_ch3
# 用瀏覽器開啟
start ch3_interactive_EN.html   # Windows
open ch3_interactive_EN.html    # macOS
xdg-open ch3_interactive_EN.html  # Linux
```

---

## 技術資訊 / Technical Notes

- 數學公式渲染：KaTeX（CDN 載入，需網路連線）
- 圖表：SVG（脈衝 / 三角 / 階梯輸入示意圖、Figure 3-1 根位置圖）+ Canvas（Example 3.4 時域響應曲線）
- 翻轉卡片：CSS 3D transform，點擊翻轉顯示正反面
- 純前端，無需後端伺服器
