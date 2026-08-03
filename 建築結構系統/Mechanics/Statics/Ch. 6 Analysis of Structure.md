## Three broad categories of Structure

#### 1. Trusses
- Two-force member
- ==Tension== or ==Compression==
#### 2. Frames
- multi-force member
#### 3. Machines

## Frame

1. 先找two-force members，因其必定延connection方向受力。
2. 如何計算靜定度？
	- free body = 3 equations
	- connection(pin) = 2 unknown force
	- support → 
		Hinge = 2 unknown force
		Roller = 1 unknown force

## Truss - Zero Force Member

![[Truss Zero Force Member.png|400]]

- Truss → 2 force members（Tension or Compression）
	- Tension（拉力）：桿件兩端箭頭指向外（← →）
	- Compression（壓力）：桿件兩端箭頭指向內（→ ←）
- Zero force member：
	- 若某接點（joint）沒有外力作用，且僅由兩不共線（non-collinear）桿件相接，則該點：
		- $F_y=0$
		- $F_c=0$
	- → 該兩桿件皆為 zero force member，取決於外力作用點。

## 6.10 Frame — Worked Example (Static Determinacy)

![[Frame Static Determinacy Example.png|300]]

- 分析步驟
	1. 先找 two-force member（如 BE），因其必定沿桿件方向受力。
	2. 如何計算靜定度？
		- 內力（構件本身）
			① 3 個構件（AD、BE、CF，獨立、無相依的 free body）→ $3×3=9$ equations
				（平面 2D → equations = 3 → $F_{x,y}=0$、$M_z=0$）
			② 3 個 connection（pin，at B、C、E）→ $3×2=6$ unknown force
		- 外力
			③ 2 個 support（1 Hinge at A + 1 Cable at G）→ $1×2+1×1=3$ unknowns
	3. $9$ equations 解 $9$ unknowns $=0$，靜定結構。（外力需不全平行、亦不共點）

## Frames & Machines

- 由數個構件與元件（member & component）以 pin 或其他方式連接組成。
- two-force members or multi-force members.
- each member → free body → 3 equations
- connection pin → 2 unknowns
- support
	- Hinge → 2 unknowns
	- Roller → 1 unknown
- $\Rightarrow$ unknowns
	- $>$ equations → statically indeterminate（靜不定）
	- $<$ equations → nonrigid（不穩定、非剛體）
	- $=$ equations → statically determinate（靜定）