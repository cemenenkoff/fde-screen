# FDE Technical Screen

## Objective
- Write a ***function*** to ***sort*** packages into stacks ***by volume*** and ***mass***.

## Rules
- A ***package*** is
  - a rectangular prism with volume defined by $V=xyz$.
  - roughly constant density with mass defined by $m=\rho V$.
  - ***bulky*** $(\beta)$ if
    - $V\geq10^6\mathrm{cm}^3$ ***or***
    - $\max(x,y,z)\geq150\mathrm{cm}$.
  - ***heavy*** $(\eta)$ if
    - $m\geq20\mathrm{kg}$.
- A stack is
  - ***STANDARD*** if $\neg\beta\land\neg\eta = \neg(\beta\lor\eta)$
  - ***SPECIAL*** if $\beta\lor\eta$
  - ***REJECTED*** if $\beta\land\eta$