Scalar-Transport-Model
===
Scalar transport sover can be enbeded in SOWFA solver to evaluate wake recovry in wind turbine flows.

## Paper
Qinghong Tang, Yifan Sun, Yuxin Wu, Mengshang Zhao, Changhua Li, Peiyao Duan, Junfu Lyu. Wake characteristics and scalar transport equation for energy recovery analysis under different tip speed ratio conditions[J]. Renewable Energy, 256(2026), 124409. https://doi.org/10.1016/j.renene.2025.124409

## Compile the scalarTransport solver
The solver is located at `pisoFoamTurbine.ALMAdvanced.scalarTransport`.
As for SOWFA simulation, put `pisoFoamTurbine.ALMAdvanced.scalarTransport` into `applications\solvers\incompressible\windEnergy\`. And then use `wmake` to compile solver.

## Setup of case
As for folder `Example_Case`, put file `sPhi` in your `0` folder, and copy parameters of file `transportProperties` and then add them into your `transportProperties` file, and set `fvSchemes` as well as `fvSolution` of your case byu reference of two files in folder `system`.
