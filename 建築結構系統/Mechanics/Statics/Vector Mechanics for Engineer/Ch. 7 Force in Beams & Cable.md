![[shear force and bending mement.png|300]]

- Axial Force（F）：軸力，沿／平行桿件軸方向受力。
- Shear Force（V）：剪力，垂直軸方向。
- Bending Moment（M）：彎矩

## Force in Beams & Cables

- Beam：承受集中載重（P）或分布載重（w(x)）
- Cable：承受分布之垂直載重

- 於任一斷面切開，取一側 free body：
	- $\sum F_x=0 \rightarrow V$（shear force，剪力）
	- $\sum F_y=0 \rightarrow F$（axial force，軸力）
	- $\sum M_j=0 \rightarrow M$（bending moment，彎矩）

## Force in Beams

![[Pasted image 20260801002927.png]]

- $V$ = shear force（剪力）
- $M$ = bending moment（彎矩）

### Sign Convention（正負號規定）

- 正 M：$\underbrace{\smile}_{+}$，樑段呈上凹（concave up），左端 M 逆時針、右端 M 順時針；V：左端向上、右端向下
- 負 M：$\overbrace{\frown}^{-}$，樑段呈下凹（concave down），符號相反

## 7.5 Shear Force and Bending Moment Diagrams

- 樑任一點 P 之內力：從支承端取斷面切開至 P 點，以 free body 求解該斷面之 $V$、$M$（必要時含 $F$）。
- Definition：切斷面兩側，內力方向相反（作用力與反作用力），正方向依上述 sign convention 決定。

### Example（simply supported beam，跨中點載重 P）

![[Pasted image 20260801003150.png]]

- $x$：$A$ 到 $C$，即 $0$ 到 $\dfrac{L}{2}$
	- $\sum F_y=0$：$V=\dfrac{P}{2}$
	- $\sum M=0$：$M=\dfrac{P\cdot x}{2}$
- $x$：$C$ 到 $B$，即 $\dfrac{L}{2}$ 到 $L$
	- $\sum F_y=0$：$V=-\dfrac{P}{2}$（即方向向上為 $\dfrac P2$，但正負依座標系為負）
	- $\sum M=0$：$\dfrac{P}{2}\cdot x-P\left(x-\dfrac{L}{2}\right)=M$
	- $\Rightarrow M=\dfrac{P(L-x)}{2}$

## 7.6 Relation Between W, V & M

- 取樑上一微小段 $\Delta x$（分布載重 $w(x)$ 作用其上）：
	- $\sum F_y=0$：$V-w\Delta x-(V+\Delta V)=0$
		- $\Delta V=-w\Delta x$
		- $\dfrac{\Delta V}{\Delta x}=-w$
		- $\Delta x\to0$：$\dfrac{dV}{dx}=-w$　（= slope of V-diagram）
	- 對分布載重積分：
		- $\displaystyle\int_{x_C}^{x_D}dV=-\int_C^D w\,dx$
		- $V_D-V_C=-($area under the load curve between C & D$)$
	- 對集中載重 $P$（$\Delta x\to0$）：
		- $\dfrac{dV}{dx}=-w=-\infty$（剪力圖在集中載重處產生突變）
	- $\sum M_{C'}=0$：$(M+\Delta M)-M-V\Delta x+w\Delta x\cdot\dfrac{\Delta x}{2}=0$
		- $\dfrac{\Delta M}{\Delta x}=V-w\Delta x\cdot\dfrac12$
		- $\Delta x\to0$：$\dfrac{dM}{dx}=V$　（= slope of M-diagram）
	- $\displaystyle\int_C^D dM=\int_C^D V\,dx$
		- $M_D-M_C=$ area under shear curve between C & D

### Conclusion

- Ⅰ. $\dfrac{dV}{dx}=V'(x)=-w$
- Ⅱ. $\dfrac{dM}{dx}=M'(x)=V$
