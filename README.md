# Apps
The main app entry point is called `APP`.

## APP/XINDA (To Avoid Confusion with General Name APP)
A system which compiles and does something like `FUNC` and also a menuing app is within this file.
`XINDA` is a wrapper to call indirect code and manage state saving. There are some `XITn` calls
to return datums (tail call optimization encouraged), and `DRPX` to "consume" input datums.
The menus are as follows
 * `FRAC` fractions, units `ENTER`, numerator `ENTER`, denominator then 1 of 4 functions. The first and last
 functions are store as and recall/display from respectively. The "divide plus" notation of the RPN decimal
 of `Z + Y / X`.
   * `÷+→`, `÷++`, `÷+-`, `÷+×`, `÷+÷`, `→÷+`.
 * `INTS` integer functions.
   * `GCD`, `LCM`.
 * `PDFS` beta and probability density functions.
   * `BETA` beta function.

# Equations for Solver
Some of the following equations can or are used to provide `APP` functions.

## WAAL
Universal gas law solver with constants `a` and `b` for better solutions.

## TVM
Time Value Money with `B/E` boolean. Beginning payments is one. Ending payments is zero. 

## CSRL
The cosine rule. Set `A` to 90 degrees for Pythagoras.

# Equations for Integrate
Some of the following equations can or are used to provide `APP` functions.
All equations are stored in the form `differential - ∫ = 0` so can be evaluated in
the solver when not required to be integrated. This requires the addition of
`∫ * (ULIM - LLIM)` after integration, or setting `∫` to zero.

The `∫` variable is named as the integral symbol by `MVAR "∫"`, even though it's the
differential of the integral when used as a variable for the solver.

## DIST
Various things to integrate for statistics distributions.
  * `EULI`, `NORMI`, `FDISTI`, `CHI2I`, `BETAI`, `LOGDI`, `STUTI`, `WEIBI`, `EXPDI`.

# XTRAS
Various extra bits found elsewhere.

