# Planning Report



## Abstract




## Block Flow Diagram





## Reaction Kinetics Data <br>
Reaction 1: <br>
<img src="https://latex.codecogs.com/gif.latex?C_{3}H_{6}(propylene)\;&space;&plus;\;&space;C_6H_6(benzene)\;&space;\overset{k1}{\rightarrow}\;&space;C_9H_{12}(cumene)" title="C_{3}H_{6}(propylene)\; +\; C_6H_6(benzene)\; \overset{k1}{\rightarrow}\; C_9H_{12}(cumene)" /></a> <br>
<img src="https://latex.codecogs.com/gif.latex?r_1\;&space;=\;&space;k_1c_pc_b&space;\;&space;[=]&space;\;&space;\frac{mol}{g_{cat}sec}" title="r_1\; =\; k_1c_pc_b \; [=] \; \frac{mol}{g_{cat}sec}" /></a> <br>
where cp is the concentration of propylene and cb is the concentration of benzene. <br>
<img src="https://latex.codecogs.com/gif.latex?k_1\;&space;=\;&space;3.5*10^{4}exp(\frac{-24.9}{RT})" title="k_1\; =\; 3.5*10^{4}exp(\frac{-24.9}{RT})" /></a> <br>

Reaction 2: <br>
<img src="https://latex.codecogs.com/gif.latex?C_{3}H_{6}(propylene)\;&space;&plus;\;&space;C_9H_{12}(cumene)\;&space;\overset{k2}{\rightarrow}\;&space;C_{12}H_{18}(p-diisopropyl&space;benzene)" title="C_{3}H_{6}(propylene)\; +\; C_9H_{12}(cumene)\; \overset{k2}{\rightarrow}\; C_{12}H_{18}(p-diisopropyl benzene)" /></a> <br>
<img src="https://latex.codecogs.com/gif.latex?r_2\;&space;=\;&space;k_2c_pc_c&space;\;&space;[=]&space;\;&space;\frac{mol}{g_{cat}sec}" title="r_2\; =\; k_2c_pc_c \; [=] \; \frac{mol}{g_{cat}sec}" /></a> <br>
where cp is the concentration of propylene and cc is the concentration of cumene. <br>
<img src="https://latex.codecogs.com/gif.latex?k_2\;&space;=\;&space;2.9*10^{6}exp(\frac{-35.08}{RT})" title="k_2\; =\; 2.9*10^{6}exp(\frac{-35.08}{RT})" /></a> <br>

## Thermodynamics Package and Additional Data

Benzene, propylene, propane, cumene, and P-diisopropyl benzene are the components in our system. All these compounds are hydrocarbons making the Soave-Redlich-Kwong (SRK) thermodynamic model the best fit for our system. SRK is commonly used for systems containing hydrocarbons and light gases. All these compounds are non-polar because they contain only carbon and hydrogen meaning interactions between these compounds (particularly in the liquid phase) will most likely be ideal and not require liquid phase activity coefficients. If we find it hard to model this system in ASPEN and achieve stream conditions close to the table in the project description, then we may choose a different thermodynamic model that may better take these interactions into account (e.g. a modified SRK).


## Design Cost Estimate
