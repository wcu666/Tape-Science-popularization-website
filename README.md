# 探討牽引速率對透明膠帶剝離時條紋形成之影響
> **Investigation Influences of Pulling Speed on Stripe Pattern Formation of Peeled Tape**

🏫 **國立中正大學 ｜ 基礎物理實驗學 2B 期末專題 ｜ 2026 物理教育聯合會議（大專生組）**

這是一個探討「撕透明膠帶」日常現象背後物理機制的專題計畫。本專案不僅包含實驗數據與力學分析，更開發了網頁版的**互動物理模擬器**，以視覺化方式呈現高分子黏膠在不同剝離速率下的動態行為。

---

## 📖 專案簡介 (Introduction)

撕開透明膠帶時，膠帶表面常呈現「白色條紋（White Zone）」與「透明條紋（Transparent Zone）」交錯的現象。當拉扯速率改變時，撕裂阻力、聲音高低，以及條紋分布距離都會隨之變化。本研究旨在建立一套能穩定且定量控制牽引速率的實驗系統，探討：
1. 牽引速率對膠帶剝離過程中臨界拉力與動態張力變化的影響。
2. 定量分析不同牽引速率下，膠帶上條紋特徵（White/Transparent Zone）的演變規律。

## 🔬 物理原理 (Physics Theory)

本研究透過宏觀動力學與微觀高分子物理來解釋**黏滑不穩定性 (Stick-Slip Instability)**：

*   **巨觀動力學：彈簧-滑塊模型 (Spring-Block Model)**
    $$m\ddot{x}=k(vt-x)-F(\dot{x})$$
    將膠帶視為彈簧，剝離交界點視為滑塊，系統在「累積彈性位能（Stick）」與「瞬間滑移（Slip）」間週期性切換。
*   **微觀機制：底波拉數 (Deborah Number, $De$)**
    *   **低速區 ($De \ll 1$)**：高分子有時間鬆弛，處於「橡膠態」，產生巨觀拉絲與白色條紋。
    *   **高速區 ($De \gg 1$)**：牽引時間極短，黏膠被迫進入「玻璃態」，發生脆性斷裂，留下透明平坦區；同時伴隨「黏彈硬化效應 (Viscoelastic stiffening)」使剝離阻力隨速率上升。

## 🛠️ 實驗裝置 (Experimental Setup)

我們自行設計並架設了**三滑輪牽引實驗系統**：
*   **動力控制**：利用微控器與步進馬達，精準控制膠帶剝離的牽引速率。
*   **張力量測**：結合拉力感測器，即時擷取剝離過程中的微小動態張力變化（F-t 曲線）。
*   **穩定機構**：透過一組動滑輪與兩組定滑輪，確保受力均勻與牽引方向穩定。

## 📊 核心結論 (Key Findings)

1.  **三大動態區域劃分**：牽引速率與剝離拉力關係可分為「極慢速區（平穩）」、「不穩定區（劇烈震盪）」與「快速區（拉力上升）」。
2.  **條紋間距規律 ($\lambda = \lambda_{stick} + \lambda_{slip}$)**：
    *   **白色條紋 ($\lambda_{stick}$)** 隨速率遞減。
    *   **透明條紋 ($\lambda_{slip}$)** 隨速率遞增。
    *   **整體條紋間距 ($\lambda$)** 隨速率遞減，證實了「撕膠帶速度越快，殘留的條紋越細密」的現象。

## 💻 網頁互動模擬器 (Interactive Simulator)

本專案內建了用以展示實驗結果的 Web 模擬器，讓使用者能夠親自操作：
*   **調整牽引速度 (Pulling Speed)**
*   **即時觀察張力-時間波形變化**
*   **視覺化膠帶生成的條紋演變**

> **使用方法**：直接在瀏覽器中開啟 `index.html`，並切換至「7. 互動模擬器」頁籤，或單獨開啟 `simulator.html` 進行體驗。

## 👥 團隊資訊 (Team)

*   **研究作者**：蔡政達、吳昌育 (Web Developer)、張中睿
*   **指導教授**：段必輝 教授 (Prof. Pi-Hui Tuan)
*   **機構/活動**：國立中正大學 / 2026 物理教育聯合會議

## 📚 參考資料 (References)

1. Grzelka, M., et al. (2022). *Transition from viscoelastic to fracture-like peeling of pressure-sensitive adhesives.* Soft Matter.
2. Everaerts, A. I., & Clemens, L. M. (2002). *Chapter 11 - Pressure sensitive adhesives.* Adhesion Science and Engineering.

---
*© 2026 Chang-Yu Wu, Zheng-Da Tsai, and Zhung-Rui Zhang. All rights reserved.*
