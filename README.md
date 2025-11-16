# PDE_FiniteElement

# Finite Element Methods Project

This README outlines several PDE problems solved using the finite element method (FEM) with piecewise linear basis functions. Each section describes the equation, boundary/initial conditions, and relevant formulation details.

---

## 1. Poisson Equation (Dirichlet Boundary Conditions)

Solve the 1D Poisson equation on the interval (0,1):

```
-u'' = 1,   0 < x < 1
u(0) = 0
u(1) = 0
```

Use a finite element method with piecewise linear basis functions. method with piecewise linear basis functions.

---

## 2. Elliptic Equation (Neumann Boundary Conditions)

Solve the equation on the domain (0, π/2):

```
-u'' + u = 1,   x ∈ (0, π/2)
u'(0) = 1
u'(π/2) = 1
```

Use a finite element method with piecewise linear basis functions.

---

## 3. Non-Homogeneous Diffusion Equation

Solve the diffusion equation:

```
u_t - u_xx = 1,   x ∈ (0,1),   t ∈ (0,1)
u(0,t) = 0
u(1,t) = 0
u(x,0) = 0
```

Use a finite element spatial discretization with piecewise linear basis functions.

---

## 4. Second-Order Hyperbolic Equation

Solve the wave-type equation:

```
u_tt - u_xx = 1,   x ∈ (0,1),   t ∈ (0,1)
u(0,t) = 0
u(1,t) = 0
u(x,0) = 1
u_t(x,0) = 0
```

Use a finite element spatial discretization with piecewise linear basis functions.

---

## 5. Biharmonic-Type Equation (Variational Interpretation)

Consider:

```
d^4u/dx^4 = f,   0 < x < 1
u(0) = 0
u'(0) = 0
u(1) = 0
nu'(1) = 0
```

Variational form:

```
(u'' , v'') = (f, v)   for all v ∈ W
```

where the function space is:

```
W = { v : v, v' continuous on [0,1],
      v'' piecewise continuous,
      v(0)=v'(0)=v(1)=v'(1)=0 }
```


