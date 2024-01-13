# Apps
The main app entry point is called `APP`.

## APP/XINDA (To Avoid Confusion with General Name APP)
A system which compiles and does something like `FUNC` and also a menuing app is within this file.
`XINDA` is a wrapper to call indirect code and manage state saving. There are some `XITn` calls
to return datums (tail call optimization encouraged), and `DRPX` to "consume" input datums.
The menus are as follows
 * `FRAC` fractions, units `ENTER`, numerator `ENTER`, denominator then 1 of 4 functions. The first and last
 functions are store as and recall/display from respectively.
 * `INTS` integer functions `GCD`.

# Equations for Solver
Some of the following equations can or are used to provide `APP` functions.

## WAAL
Universal gas law solver with constants `a` and `b` for better solutions.

## TVM
Time Value Money with `B/E` boolean. Begin is zero. End is one. 

# Equations for Integrate
Some of the following equations can or are used to provide `APP` functions.

