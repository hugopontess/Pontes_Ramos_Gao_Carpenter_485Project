# Planning Report



## Abstract <br>
The purpose of project 6 in Turton et. al is to design a cumene production facility that produces 100,000 metric tons per year. In such, we are asked to design a grassroots cumene process using benzene and propylene. This will be done using a new catalyst, for which the reaction kinetics are included in this report. The deliverables for this project will be an optimized preliminary design of the plant and an economic evaluation of the process. The two inputs are benzene and propylene in order to produce cumene. However, there is a side reaction between propylene and cumene that produces p-diisopropyl benzene, and the remaining benzene, propylene, propane, and some cumene exit as fuel gas. The process incudes a catalytic reaction followed by a separator that purges propylene, benzene, and propane as fuel gas, while also recycles that stream into the feed preparation. There is also a cumene separator that gives the pure product, separating it from the side reaction product. <br>



## Block Flow Diagram
![BFD](BFD2.JPG)
Assuming an overall conversion of 90% for the cumene, 3% for the p-diisopropyl benzene, stoichiometric feed, and a perfect separation process, the mass balance for the inputs and outputs will look like this: <br>
mass flow rate of benzene into process - 72,210 metric tons/year <br>
mass flow rate of propylene into process - 35,011 metric tons/year <br>
mass flow rate of cumene out of process - 100,000 metric tons/year <br>
mass flow rate of p-diisopropyl benzene out of process - 4500 metric tons/year <br>
mass flow rate of fuel gas - 2721 metric tons/year <br>


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
Price of benzene (textbook): $0.919/kg --> cost per year is 72,210 tons * $0.919/kg * 1000 kg/ton = $66.4 mil <br>
Price of propylene (textbook): $1.444/kg --> cost per year is 35,011 tons * $1.444/kg * 1000 kg/ton = $50.6 mil <br>
Price of cumene (online at https://www.intratec.us/chemical-markets/cumene-price): $1210/ton --> earnings per year are 100,000 tons * $1210/ton = $121 mil <br>
p-diisopropylbenzene, treating as a fuel: heat of combustion = 6.82 GJ/kmol, MW = 162.3 kg/kmol, energy cost = $2.50/GJ --> earnings per year are 4500 tons * 1000 kg/ton * 1/162.3 kmol/kg * 6.82 GJ/kmol * $2.50/GJ = $0.5 mil <br>
Fuel gas: Assuming fuel gas has similar heat of comubstion, and MW to p-diisopropylbenzene --> $0.3 mil <br>
Total net chemical cost: 4.8 mil <br>
The positive net chemical cost is positive, suggesting this plant may be feasible.
