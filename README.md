# PDE_FiniteElement

# Finite Element Methods Project

This README outlines several PDE problems solved using the finite element method (FEM) with piecewise linear basis functions. Each section describes the equation, boundary/initial conditions, and relevant formulation details.

---

## 1. Poisson Equation (Dirichlet Boundary Conditions)

Solve the 1D Poisson equation on the interval ((0,1)):

[-u'' = 1, \quad 0 < x < 1]

with Dirichlet boundary conditions:

[u(0) = 0, \quad u(1) = 0.]

Use a finite element method with piecewise linear basis functions.

---

## 2. Elliptic Equation (Neumann Boundary Conditions)

Solve the equation on the domain ((0, \pi/2)):

[-u'' + u = 1, \quad x \in (0, \tfrac{\pi}{2})]

with Neumann boundary conditions:

[u'(0) = 1, \quad u'\left(\tfrac{\pi}{2}\right) = 1.]

Use a finite element method with piecewise linear basis functions.

---

## 3. Non-Homogeneous Diffusion Equation

Solve the diffusion equation:

[u_t - u_{xx} = 1, \quad x \in (0,1),; t \in (0,1),]

with boundary and initial conditions:

* (u(0,t) = 0)
* (u(1,t) = 0)
* (u(x,0) = 0)

Use a finite element spatial discretization with piecewise linear basis functions.

---

## 4. Second-Order Hyperbolic Equation

Solve the wave-type equation:

[u_{tt} - u_{xx} = 1, \quad x \in (0,1),; t \in (0,1),]

with boundary conditions:

* (u(0,t) = 0)
* (u(1,t) = 0)

and initial conditions:

* (u(x,0) = 1)
* (\dot{u}(x,0) = 0)

Use a finite element spatial discretization with piecewise linear basis functions.

---

## 5. Biharmonic-Type Equation (Variational Interpretation)

Consider:

[\frac{d^4u}{dx^4} = f, \quad 0 < x < 1,]

with boundary conditions:

[u(0) = 0,; u'(0) = 0,; u(1) = 0,; u'(1) = 0.]

Show the problem has the following variational form:

Find (u \in W) such that

[(u'' , v'') = (f, v), \quad \forall v \in W,]

where the function space is

[
W = {v: v, v' \text{ continuous on } [0,1],; v'' \text{ piecewise continuous},; v(0)=v'(0)=v(1)=v'(1)=0}.
]

---

This README summarizes the mathematical formulations for each PDE and the corresponding FEM setup.
