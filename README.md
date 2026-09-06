# R&D / AI Assignment – Parametric Curve Fitting

## Final Result

The unknown parameters are:

\[
\boxed{\theta = 30^\circ}
\]

\[
\boxed{M = 0.03}
\]

\[
\boxed{X = 55}
\]

## Parametric Equation

The original parametric equation is:

\[
x = t\cos(\theta)
- e^{M|t|}\sin(0.3t)\sin(\theta)
+ X
\]

\[
y = 42+t\sin(\theta)
+e^{M|t|}\sin(0.3t)\cos(\theta)
\]

with:

\[
6<t<60
\]

## Equation With Estimated Parameters

Substituting the estimated values:

\[
x=t\cos(30^\circ)
-e^{0.03|t|}\sin(0.3t)\sin(30^\circ)+55
\]

\[
y=42+t\sin(30^\circ)
+e^{0.03|t|}\sin(0.3t)\cos(30^\circ)
\]

where:

\[
6<t<60
\]

## Method

The parameters were estimated using a mathematical transformation
of the provided XY points followed by Differential Evolution
optimization.

The final fitted curve was then compared with the provided data
using L1 distance and uniform sampling.


## Files

- `R&D_AI_Parametric_Curve_Fitting.ipynb` – Python implementation
- `xy_data.csv` – Provided dataset

## Desmos Visualization

The final parametric curve using the estimated parameters can be viewed
interactively in Desmos:

[View the Desmos Graph](https://www.desmos.com/calculator/vey7shuv0r)
