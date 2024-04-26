Implementing a short matlab script to quickly solve for missing traction-separation variables for cohesive damage. 


###Solving for Fracture Energy and Stiffness
Begin by inputting the required variables into [SolveforKn_Gc](https://github.com/midmidmidmid/TractionSeparation/blob/main/SolveforKn_Gc), in this case your maximum separation, damage separation, and maximum traction.

![Assign Variables](https://github.com/midmidmidmid/TractionSeparation/blob/main/plots/Matlab_Variables.png)

The Kn is calculated as the slope from the origin to the apex point. The fracture energy is the triangle area.

![Calculations](https://github.com/midmidmidmid/TractionSeparation/blob/main/plots/calcs.png)

The following plot is made:

![Plot](https://github.com/midmidmidmid/TractionSeparation/blob/main/plots/Matlab_TractionSeparation.png)

You can therefore vary the damage separation to parametrize along this variable:

![DamSepPlot](https://github.com/midmidmidmid/TractionSeparation/blob/main/plots/combinedplots4.png)


Similarly this can be done for the maximum traction: 

![MaxTracPlot](https://github.com/midmidmidmid/TractionSeparation/blob/main/plots/combinedplots2.png)


Through [SolveforMaxSep_DamageSep](https://github.com/midmidmidmid/TractionSeparation/blob/main/SolveforMaxSep_DamageSep) you can solve for the max separation and damage separation. These results are in red to differentiate. 

Solely changing Gc we get:

![GcChanged](https://github.com/midmidmidmid/TractionSeparation/blob/main/plots/combinedplots5.png)

and changing Kn we get:

![Knchanged](https://github.com/midmidmidmid/TractionSeparation/blob/main/plots/combinedplots6.png)
