---
up: "[[architectureData/建築結構系統/結構系統概論/CH. 0 Contents]]"
---

## 剪應力・撓曲應力・扭應力

![[剪應力撓曲應力扭應力.png|400]]

### 剪應力

- 純剪力元素中，一組對角線受拉、另一組對角線受壓（約45°方向），此即主應力方向。
- RC梁受剪力時，斜向裂縫沿約45°方向發展。

### 撓曲應力（bending stress）

- 以中性軸 N.A.（neutral axis）為界，分壓應力側、張應力側。
- 一旦龜裂，張應力側改由鋼筋（steel）承受，壓應力側仍由混凝土（RC）承受。
- $M$＝彎矩；隨外力增大、達塑性階段，斷面應力分佈由三角形漸趨向矩形（塑性應力分佈）。

### 扭應力（torsional stress）

- 裂縫走向約45°，呈連續螺旋狀。
- 斷面之剪應力分佈不均；長寬比 $L≥2W$ 時較易因抗扭力產生開裂。

## 基本應力公式

![[基本應力公式.png|400]]

- 張應力：

$$
F_t<0.6×F_u（極限抗拉應力）
$$

<span style="color:#d32f2f">（⚠️ 建議查證：常見容許應力設計法中，容許張應力多定義為 $F_t=0.6F_y$（依降伏強度 $F_y$計算），淨斷面另有 $F_t=0.5F_u$（依極限強度）之規定；筆記中寫成「$0.6×F_u$」，建議核對鋼結構設計規範原文，確認是否誤植）</span>

- Poisson's ratio：

$$
\nu=-\frac{\text{lateral strain }\varepsilon'}{\text{axial strain }\varepsilon}
$$

	- $0.25≤\nu≤0.35$
- 壓應力／挫屈：
	- 挫屈載重（Euler公式）：$P_{cr}=\dfrac{\pi^2EI}{(kl)^2}$
	- 挫屈應力：$\sigma_{cr}=\dfrac{P_{cr}}{A}$
	- 容許撓曲應力：約 $0.60\sim0.75F_y$
	- $\sigma=\dfrac{Ey}{r}$（$r$＝曲率半徑，$y$＝距中性軸距離）
- 剪應力：
	- 剪應變 $\gamma=\dfrac{剪應力\ \tau}{剪力彈性係數\ G}$
	- $G=\dfrac{E}{2(1+\mu)}$，$\mu=$Poisson's ratio
