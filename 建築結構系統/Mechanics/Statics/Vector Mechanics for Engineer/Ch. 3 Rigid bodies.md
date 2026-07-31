-  Non-deformable
- Transmissibility moment about point/axis
- External & Internal Force

	## Vector Product

![[Vector Product.png|300]]

### Dot Product(內積)

- $\overrightarrow{Q}·\overrightarrow{P}=|Q|\cosθ|P|$ = Q在P的投影長度 × P的長度
### Cross Product(外積)

- $\overrightarrow{V}=\overrightarrow{P}×\overrightarrow{Q}$   ;   $\overrightarrow{V}\perp\overrightarrow{P}$    ;   $\overrightarrow{V}\perp\overrightarrow{Q}$
	-  $V=P×Q\sinθ$ = areaOPAQ = length of V
	- $\overrightarrow{P}×\overrightarrow{Q}=-\overrightarrow{Q}×\overrightarrow{P}$
	- $\overrightarrow{P}×(\overrightarrow{Q_1}+\overrightarrow{Q_2})=\overrightarrow{P}×\overrightarrow{Q_1}+\overrightarrow{P}×\overrightarrow{Q_2}$
	- $(\overrightarrow{P}×\overrightarrow{Q})×\overrightarrow{S}\neq\overrightarrow{P}×(\overrightarrow{Q}×\overrightarrow{S})$

- $\overrightarrow{i}×\overrightarrow{i}=\overrightarrow{j}×\overrightarrow{j}=\overrightarrow{k}×\overrightarrow{k}=0$
	- $\overrightarrow{i}×\overrightarrow{j}=\overrightarrow{k}$
	- $\overrightarrow{j}×\overrightarrow{k}=\overrightarrow{i}$
	- $\overrightarrow{k}×\overrightarrow{i}=\overrightarrow{j}$

- $\begin{aligned}\overrightarrow{V}&=\overrightarrow{P}×\overrightarrow{Q}\\&=(P_x\overrightarrow{i}+P_y\overrightarrow{j}+P_z\overrightarrow{k})×(P_x\overrightarrow{i}+P_y\overrightarrow{j}+P_z\overrightarrow{k})\\&=\begin{vmatrix}\overrightarrow{i}&\overrightarrow{j}&\overrightarrow{k}\\P_x&P_y&P_z\\Q_x&Q_y&Q_z\end{vmatrix}\\&=(P_yQ_z-P_zQ_y)\overrightarrow{i}+(P_zQ_x-P_xQ_z)\overrightarrow{j}+(P_xQ_y-P_yQ_x)\overrightarrow{k}\end{aligned}$

## Moment of a Force about a Point

![[Moment of a Force about a Point.png|300]]

- $\overrightarrow{M_0}\equiv\overrightarrow{r}×\overrightarrow{F}$
- $M_0=r×F\sin\theta=F×d$
- for 2D 
	- $z = 0$   ;   $f_z = 0$
	- $\overrightarrow{M}=\begin{vmatrix}\overrightarrow{i}&\overrightarrow{j}&\overrightarrow{k}\\x&y&0\\F_x&F_y&0\end{vmatrix}=M_z\overrightarrow{k}$


## Moment of a Force about a Axis

![[Moment of a Force about a Axis.png|300]]

- $\overrightarrow{M_0}=\overrightarrow{r}×\overrightarrow{F}$
	- $\begin{aligned}M_{OL}&=\overrightarrow{λ_{OL}}·\overrightarrow{M_0}\\&=\overrightarrow{λ_{OL}}·(\overrightarrow{r}×\overrightarrow{F})\\&=\begin{vmatrix}\overrightarrow{λ_x}&\overrightarrow{λ_y}&\overrightarrow{λ_z}\\r_x&r_y&r_z\\F_x&F_y&F_z\end{vmatrix}\end{aligned}$
	-  $\overrightarrow{r}=\overrightarrow{r_1}×\overrightarrow{r_2}$ 
	- $\overrightarrow{F}=\overrightarrow{F_1}×\overrightarrow{F_2}$    ;$\overrightarrow{F_1}\parallel{OL},\overrightarrow{F_2}$ on the plane
	- $\begin{aligned}M_{OL}&=\overrightarrow{λ}·\overrightarrow{M_0}\\&=\overrightarrow{λ}·(\overrightarrow{r}×\overrightarrow{F})\\&=\overrightarrow{λ}·[(\overrightarrow{r_1}+\overrightarrow{r_2})×(\overrightarrow{F_1}+\overrightarrow{F_2})]\\&=\overrightarrow{λ}·[(\overrightarrow{r_1}×\overrightarrow{F_1})+(\overrightarrow{r_1}+\overrightarrow{F_2})+(\overrightarrow{r_2}×\overrightarrow{F_1})+(\overrightarrow{r_2}+\overrightarrow{F_2})]\end{aligned}$
		   $\because\overrightarrow{λ}\parallel\overrightarrow{r_1}$   and  $\overrightarrow{F_1}$
		   $\therefore$ 第一、二、三項為0，且$\overrightarrow{λ}$為1
		   $=\overrightarrow{λ}·(\overrightarrow{r_2}×\overrightarrow{F_2})$
		   $=\left|(\overrightarrow{r_2}×\overrightarrow{F_2})\right|$

### Scalar Product 

![[Scalar product.png|300]]

- $\overrightarrow{P}·\overrightarrow{Q}\equiv PQ\cos\theta$
- $\overrightarrow{P}·\overrightarrow{Q}=\overrightarrow{Q}·\overrightarrow{P}$
-  $\overrightarrow{i}·\overrightarrow{i}=\overrightarrow{j}·\overrightarrow{j}=\overrightarrow{k}·\overrightarrow{k}=1$
	- $\overrightarrow{i}·\overrightarrow{i}=i×i\cos0°=1$
	- $\overrightarrow{i}·\overrightarrow{j}=i×j\cos90°=0$
- $\begin{aligned}\overrightarrow{P}·\overrightarrow{Q}&=(P_x\overrightarrow{i}+P_y\overrightarrow{j}+P_z\overrightarrow{k})·(Q_x\overrightarrow{i}+Q_y\overrightarrow{j}+Q_z\overrightarrow{k})\\&=P_xQ_x+P_yQ_y+P_ZQ_z\end{aligned}$

##### Mixed Triple Product

- Scalar triple Product, $\overrightarrow{S}×(\overrightarrow{P}·\overrightarrow{Q})$ 
- Vector triple Product, $\overrightarrow{S}×(\overrightarrow{P}×\overrightarrow{Q})$ 
##### Angle formed by  $\overrightarrow{P}·\overrightarrow{Q}$

-  $\begin{aligned}\overrightarrow{P}·\overrightarrow{Q}&= PQ\cos\theta\\&=\frac{\overrightarrow{P}·\overrightarrow{Q}}{P·Q}\end{aligned}$

##### Projection of a Vector

![[Projection of a Vector.png|300]]

- $P_{OL}=OA=P\cos\theta$
- $\begin{aligned}\overrightarrow{P}·\overrightarrow{Q}&= PQ\cos\theta\\&=P_{OA}·Q\end{aligned}$

## Force of Couple

##### Moment of Couple

![[The moment M of the couple.png|300]]

- $\begin{aligned}\overrightarrow{M}&=(\overrightarrow{r_A}×\overrightarrow{F})+(\overrightarrow{r_B}×\overrightarrow{-F})\\&=(\overrightarrow{r_A}-\overrightarrow{r_B})×\overrightarrow{F}\\&=\overrightarrow{r}×\overrightarrow{F}\end{aligned}$
- $\begin{aligned}M_0&=r·\sin\theta·F\\&=d·F\end{aligned}$

## System of Force → one Force + one Couple

![[截圖 2024-08-27 上午10.29.13.png|400]]

- $\begin{aligned}\overrightarrow{R}&=\sum\overrightarrow{F}\\&=\overrightarrow{F_1}+\overrightarrow{F_2}+\overrightarrow{F_3}\end{aligned}$
- $\begin{aligned}\overrightarrow{M_0}&=(\overrightarrow{r_1}×\overrightarrow{F_1})+(\overrightarrow{r_2}×\overrightarrow{F_2})+(\overrightarrow{r_3}×\overrightarrow{F_3})\\&=\sum\overrightarrow{r}×\overrightarrow{F}\end{aligned}$

### Equivalent System of Force

### at some point 

- $\sum\overrightarrow{F}=\sum\overrightarrow{F'}$
- $\sum\overrightarrow{M_0}=\sum\overrightarrow{M_0'}$

### force couple system → single force or single couple

![[Reducing a system of forces to a force-couple system.png|400]]
##### 1. $\sum\overrightarrow{F}=0$ → single couple
##### 2. force couple system → single force

1) if $\overrightarrow{R}\perp\overrightarrow{M_0}$ → single force

	(1) concurrent force
	(2) coplanar force
	(3) parallel force

2) if  $\overrightarrow{R}$  is not $\perp\overrightarrow{M_0}$

	![[Reducing a system of forces to a wrench.png|400]]
	
	(1) Wrench

		$\begin{aligned}M_1&=\overrightarrow{M_{0}^{R}}·\overrightarrow{λ}\\&= \overrightarrow{M_{0}^{R}}·\frac{\overrightarrow{R}}{R}\end{aligned}$
	
	(2) Pitch of the wrench(p)

		$\begin{aligned}p&=\frac{M_1}{R}\\&=\frac{\overrightarrow{M_{0}^{R}}·\overrightarrow{R}}{R^2}\end{aligned}$

		$M_1=p·R$
		$\overrightarrow{M_1}=p·\overrightarrow{R}$
			$\overrightarrow{M_2}=\overrightarrow{M_{0}^{R}}-\overrightarrow{M_1}$
			$\overrightarrow{R}\perp\overrightarrow{M_2}$ → single force
		