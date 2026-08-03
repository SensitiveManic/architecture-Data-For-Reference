## Chap. 9 Moment of Inertia

![[9-1.png|800]]

- $Q_x=\displaystyle\int y\,dA$
  $Q_y=\displaystyle\int x\,dA$　$\Big\}$　1st moment → centroid（形心）

- $I_x=\displaystyle\int y^2\,dA$
  $I_y=\displaystyle\int x^2\,dA$　$\Big\}$　2nd moment → mechanics of materials（材料力學）

## 9.2 Determination of Moment of Inertia of an Area by Integration

- 樑受彎矩 $M$，斷面上應力與 N.A.（neutral axis，中立軸）距離 $y$ 成正比（和 $y$ 呈線性關係）：
	- $\Delta F=ky\,\Delta A$（$\Delta F$ 對 N.A. 產生 $M$）
	- $R=\displaystyle\int dF=0$ → N.A. pass centroid（中立軸通過形心）
	- $M=\displaystyle\int y\,dF=\int y\cdot ky\,dA=k\int y^2\,dA$ → 2nd moment

## 9.3 Moment of Inertia of an Area

![[9-2.png|400]]

- $I_x\equiv\displaystyle\int y^2\,dA$，$\quad I_y\equiv\displaystyle\int x^2\,dA$

- 取垂直面積（vertical strip），$dA=dx\,dy$：
	- $dI_x=y^2\,dx\,dy=y^2\,dA$
	- $dI_y=x^2\,dx\,dy$
	- $I_x=\displaystyle\int_0^{y(x)}\int_a^b y^2\,dx\,dy$

- 取水平面積，$dA=(a-x)\,dy$：
	- $dI_x=y^2\,dA=y^2(a-x)\,dy$
	- $I_x=\displaystyle\int_0^{y(x)} y^2(a-x)\,dy$

- 取豎條，$dA=y\,dx$：
	- $dI_y=x^2\,dA=x^2\cdot y\,dx$
	- $I_y=\displaystyle\int_a^b x^2\cdot y\,dx$

## 9.4 Polar Moment of Inertia

![[9-3.png|400]]

- $r^2=x^2+y^2$
- $J_O\equiv\displaystyle\int r^2\,dA=\int x^2\,dA+\int y^2\,dA$
- $J_O=I_x+I_y$

## 9.5 Radius of Gyration of an Area（迴轉半徑）

- $I_x=\displaystyle\int y^2\,dA=k_x^2A$
- $I_y=\displaystyle\int x^2\,dA=k_y^2A$
- $J_O=I_x+I_y=k_x^2A+k_y^2A$

## 9.6 Parallel Axis Theorem

![[9-4.png|400]]

- $I_x=\displaystyle\int y^2\,dA$，$I_{x'}=\displaystyle\int y'^2\,dA$（$x'$ 為形心軸）
- $y=y'+d$

$$
\begin{aligned}I_{BB'}&=\int y^2\,dA\\&=\int(y'+d)^2\,dA\\&=\int(y'^2+2dy'+d^2)\,dA\\&=\int y'^2\,dA+2d\underbrace{\int y'\,dA}_{\text{1st moment}=0}+d^2\int dA\\&=\bar I+0+Ad^2\end{aligned}
$$

- （$\displaystyle\int y'\,dA=\bar y'A=0$，因為 $y'$ 以 $x'$ 為基準，其形心座標為 0）
- $I_{BB'}=\bar I+Ad^2$，$d>0$
- $\bar I=\bar k^2A$
- $I_{BB'}=k^2A=\bar I+Ad^2$
	- $k^2=\bar k^2+d^2$

## 9.7 Moments of Inertia of Composite Areas

- 將複雜截面分割為數個簡單幾何形狀，各自對同一軸取 $I$（必要時以 parallel axis theorem 移軸），再相加。

## 9.8 Product of Inertia

![[9-5.png|400]]

- $I_x=\displaystyle\int y^2\,dA$，$I_y=\displaystyle\int x^2\,dA$
- $I_{xy}\equiv\displaystyle\int xy\,dA$
	- 若 $x$、$y$ 其中一軸為對稱軸，則 $I_{xy}=0$（只需有一軸對稱即可）

- 對稱例：$dA(x,y)$ 與 $dA(x,-y)$ 成對出現 → $I_{xy}=\displaystyle\int xy\,dA=0$

- 平移公式（$x=x'+\bar x$，$y=y'+\bar y$，$x'y'$ 為形心軸）：

$$
\begin{aligned}I_{xy}&=\int xy\,dA=\int(x'+\bar x)(y'+\bar y)\,dA\\&=\int x'y'\,dA+\int x'\bar y\,dA+\int\bar x y'\,dA+\int\bar x\bar y\,dA\\&=\bar I_{x'y'}+\bar x\bar y A\end{aligned}
$$

## 9.9 Principal Axis and Principal Moments of Inertia

![[9-6.png|400]]

- $I_x=\displaystyle\int y^2\,dA$，$I_y=\displaystyle\int x^2\,dA$，$I_{xy}=\displaystyle\int xy\,dA$
- 座標旋轉 $\theta$：
	- $x'=x\cos\theta+y\sin\theta$
	- $y'=y\cos\theta-x\sin\theta$
	- $\sin2\theta=2\sin\theta\cos\theta$，$\cos2\theta=\cos^2\theta-\sin^2\theta$

$$
\begin{aligned}I_{x'}&=\int y'^2\,dA=\int(y\cos\theta-x\sin\theta)^2\,dA\\&=\cos^2\theta\underbrace{\int y^2\,dA}_{I_x}-2\sin\theta\cos\theta\underbrace{\int xy\,dA}_{I_{xy}}+\sin^2\theta\underbrace{\int x^2\,dA}_{I_y}\\&=I_x\cos^2\theta-2I_{xy}\sin\theta\cos\theta+I_y\sin^2\theta\\&=\dfrac{I_x+I_y}{2}+\dfrac{I_x-I_y}{2}\cos2\theta-I_{xy}\sin2\theta\end{aligned}
$$

$$
\begin{aligned}I_{y'}&=\int x'^2\,dA\\&=I_x\sin^2\theta+2I_{xy}\sin\theta\cos\theta+I_y\cos^2\theta\\&=\dfrac{I_x+I_y}{2}-\dfrac{I_x-I_y}{2}\cos2\theta+I_{xy}\sin2\theta\end{aligned}
$$

$$
\begin{aligned}I_{x'y'}&=\int x'y'\,dA\\&=I_x\sin\theta\cos\theta+I_{xy}(\cos^2\theta-\sin^2\theta)-I_y\sin\theta\cos\theta\\&=\dfrac{I_x-I_y}{2}\sin2\theta+I_{xy}\cos2\theta\end{aligned}
$$

- $I_x+I_y=I_{x'}+I_{y'}=J_O$（unvarying，旋轉不變量）

- $\left(I_{x'}-\dfrac{I_x+I_y}{2}\right)^2+I_{x'y'}^2=\left(\dfrac{I_x-I_y}{2}\right)^2+I_{xy}^2=R^2$
	$\Rightarrow(I_{x'}-I_{ave})^2+I_{x'y'}^2=R^2$

### Mohr's Circle for Moment of Inertia

![[9-7.png|400]]

- 例：矩形 $I_x=\dfrac{1}{12}bh^3$，$I_y=\dfrac{1}{12}hb^3$；若 $h>b$，則 $I_x>I_y$
- 圓心 $=I_{ave}$，半徑 $R$，橫軸 $I_x$、縱軸 $I_{x'y'}$
	- $(I_{max},0)$、$(I_{min},0)$ 為 principal moments of inertia

$$
\begin{aligned}I_{xy}&=\int xy\,dA\\&=\int(\bar x+x')(\bar y+y')\,dA\\&=\int\bar x\bar y\,dA+\int\bar xy'\,dA+\int x'\bar y\,dA+\int x'y'\,dA\end{aligned}
$$

## 9.11 Moment of Inertia of a Mass

![[9-8.png|400]]

- $\Delta I\equiv r^2\Delta m$
- $I=\displaystyle\int r^2\,dm$
- $I=k^2m$　（$k$ = radius of gyration）

- $I_y=\displaystyle\int r^2\,dm=\int(x^2+z^2)\,dm$
- $I_x=\displaystyle\int(y^2+z^2)\,dm$
- $I_z=\displaystyle\int(x^2+y^2)\,dm$

## 9.12 Parallel Axis Theorem（Mass）

![[9-9.png|400]]

- $x=\bar x+x'$，$y=\bar y+y'$，$z=\bar z+z'$

$$
\begin{aligned}I_x&=\int(y^2+z^2)\,dm\\&=\int\left[(\bar y+y')^2+(\bar z+z')^2\right]dm\\&=\int(\bar y^2+\bar z^2)\,dm+2\bar y\int y'\,dm+2\bar z\int z'\,dm+\int(y'^2+z'^2)\,dm\\&=\bar I_{x'}+m(\bar y^2+\bar z^2)\end{aligned}
$$

## 9.13 Moments of Inertia of Thin Plates

![[9-10.png|300]]

- $dm=\rho t\,dA$　（$\rho$ = 密度，$t$ = 厚度，質量比值）
- $I_{AA',mass}=\displaystyle\int r^2\,dm=\int r^2\rho t\,dA=\rho t\int r^2\,dA=\rho t\cdot I_{AA',area}$
- $I_{BB',mass}=\rho t\cdot I_{BB',area}$
- $I_{CC',mass}=\rho t\cdot I_{CC',area}=\rho t\left(I_{AA',area}+I_{BB',area}\right)$

### 矩形薄板

- $I_{AA',mass}=\rho t\cdot\dfrac{1}{12}a^3b=\dfrac{1}{12}m\cdot a^2$
- $I_{BB',mass}=\rho t\cdot\dfrac{1}{12}ab^3=\dfrac{1}{12}m\cdot b^2$
- $m=\rho\cdot ab\cdot t$
- $I_{CC'}=\dfrac{1}{12}m(a^2+b^2)$

### 圓形薄板

- $I_{AA',area}=\dfrac14\pi r^4$
- $I_{AA',mass}=\rho t\cdot\dfrac14\pi r^4=\dfrac14\pi r^2\cdot m$，其中 $m=\rho\cdot\pi r^2\cdot t$
- $I_{CC',mass}=I_{AA'}+I_{BB'}=\dfrac12mr^2$

## 9.14 Moments of Inertia of a 3D Body by Integration

- 圓錐（沿 x 軸積分為圓盤疊加）：
	- $dm=\rho\pi r^2\,dx$
	- $dI_x=\dfrac12\cdot m\cdot r^2\,dx=\dfrac12\rho\pi r^2\cdot r^2\,dx$
	- $dI_y=\left(\dfrac14 r^2\,dm\right)+dm\cdot x^2$
	- $dI_z=\left(\dfrac14 r^2\,dm\right)+dm\cdot x^2$
