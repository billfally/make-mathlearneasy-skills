# 公式速查卡（冲刺期背诵用）

按模块分组，每张"卡"是一组必须脱口而出的公式。用于生成背诵卡片与考前提问自测。

## 极限卡

- lim(x→0) sin x / x = 1；lim(x→0) (1+x)^(1/x) = e；lim (1+1/n)^n = e
- 等价无穷小（x→0）：sin x ~ tan x ~ arcsin x ~ arctan x ~ ln(1+x) ~ e^x−1 ~ x；1−cos x ~ x²/2；x−sin x ~ x³/6；tan x − x ~ x³/3；x−ln(1+x) ~ x²/2；(1+x)^α−1 ~ αx
- 1^∞ 型：lim u^v = e^{lim v(u−1)}（u→1）
- Stolz（∞/∞）：b_n 严格单增→+∞ 时 lim a_n/b_n = lim (a_{n+1}−a_n)/(b_{n+1}−b_n)

## 导数卡

- (x^α)' = αx^{α−1}；(a^x)' = a^x ln a；(ln|x|)' = 1/x
- (arcsin x)' = 1/√(1−x²)；(arctan x)' = 1/(1+x²)
- Leibniz：(uv)^(n) = Σ_{k=0}^{n} C(n,k) u^(k) v^(n−k)
- 参数方程：dy/dx = y'(t)/x'(t)；d²y/dx² = d(dy/dx)/dt ÷ x'(t)
- 变限积分：d/dx ∫_{a(x)}^{b(x)} f(t)dt = f(b(x))b'(x) − f(a(x))a'(x)

## Taylor 卡（x→0）

- e^x = 1 + x + x²/2! + x³/3! + …
- sin x = x − x³/3! + x⁵/5! − …；cos x = 1 − x²/2! + x⁴/4! − …
- ln(1+x) = x − x²/2 + x³/3 − …（−1<x≤1）
- (1+x)^α = 1 + αx + α(α−1)x²/2! + …
- 1/(1−x) = 1 + x + x² + …（|x|<1）

## 积分卡

- ∫ tan x dx = −ln|cos x|；∫ sec x dx = ln|sec x + tan x|
- ∫ dx/(x²+a²) = (1/a)arctan(x/a)；∫ dx/√(a²−x²) = arcsin(x/a)
- ∫ dx/(x²−a²) = (1/2a)ln|(x−a)/(x+a)|
- ∫ ln x dx = x ln x − x；∫ e^{ax}sin bx 型：两次分部或公式
- 点火公式：∫_0^{π/2} sin^n x dx = ∫_0^{π/2} cos^n x dx；n 偶 = (n−1)!!/n!! · π/2；n 奇 = (n−1)!!/n!!
- 区间再现：∫_0^a f(x)dx = ∫_0^a f(a−x)dx；∫_0^π x f(sin x)dx = (π/2)∫_0^π f(sin x)dx
- Cauchy–Schwarz：(∫fg)² ≤ ∫f² · ∫g²
- 反常积分基准：∫_1^∞ dx/x^p 收敛 ⇔ p>1；∫_0^1 dx/x^p 收敛 ⇔ p<1

## 多元微分卡

- 可微定义：Δz = f_x Δx + f_y Δy + o(ρ)，ρ = √(Δx²+Δy²)
- 方向导数：∂f/∂l = grad f · e_l = f_x cosα + f_y cosβ
- 梯度方向是函数值增长最快方向，|grad f| 是最大增长率
- 切平面（z = f(x,y)）：z − z₀ = f_x(x₀,y₀)(x−x₀) + f_y(x₀,y₀)(y−y₀)
- Lagrange 乘数法：∇f = λ∇φ（约束 φ = 0）

## 重积分与线面积分卡

- 极坐标：dxdy = r dr dθ；柱坐标：dV = r dr dθ dz；球坐标：dV = r² sinφ dr dφ dθ
- Green：∮_L P dx + Q dy = ∬_D (∂Q/∂x − ∂P/∂y) dxdy（L 正向）
- 路径无关（单连通）⇔ ∂Q/∂x = ∂P/∂y；原函数 u = ∫P dx + ∫Q dy 凑全微分
- Gauss：∯_Σ P dy dz + Q dz dx + R dx dy = ∭_Ω (P_x + Q_y + R_z) dV（外侧）
- Stokes：∮ P dx + Q dy + R dz = ∬ (R_y−Q_z)dy dz + (P_z−R_x)dz dx + (Q_x−P_y)dx dy
- 面积微元：dS = √(1 + z_x² + z_y²) dxdy
- div F = P_x+Q_y+R_z；rot F = ∇×F

## 级数卡

- 收敛半径：R = 1/lim |a_{n+1}/a_n| 或 1/lim ⁿ√|a_n|
- p 级数 Σ 1/n^p：收敛 ⇔ p>1；几何级数 Σ q^n：|q|<1 收敛于 1/(1−q)
- Leibniz：交错级数 u_n 单减→0 ⇒ 收敛；|余项| ≤ u_{n+1}
- 求和套路：先导后积 / 先积后导 / 套用五个基本展开
- 常用和：Σ 1/n² = π²/6；Σ (−1)^{n−1}/n = ln 2

## 常微分方程卡

- 一阶线性：y' + P(x)y = Q(x) ⇒ y = e^{−∫P}[∫Q e^{∫P}dx + C]
- Bernoulli：y' + Py = Qy^n ⇒ 令 z = y^{1−n}
- 二阶常系数齐次：特征方程 r²+pr+q = 0；两实根 / 重根 / 共轭复根三种通解
- 非齐次待定系数：f = e^{λx}P_m(x) 型，λ 是 k 重特征根则乘以 x^k
- Euler 方程：x²y'' + pxy' + qy = f(x)，令 x = e^t
