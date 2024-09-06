# Digital-Twins-for-Lung-Ventilation
We show preliminary results that use TwinBuilder for reduced order modeling (ROM) and simulation of the central upper airway tree.

Our full-order simulations are based on the inlet velocity 
V_{inlet} = amp [m/s]*sin(2*pi*freq [Hz]*t)
with amp = 0.5, 0.7, 0.9, 1.1, 1.3, 1.5 and 
     freq =0.2, 0.4, 0.6.
Therefore, we have in total 18 full-order solution snapshots.

Based on these solution snapshots, we apply ROM (TwinBuilder in Ansys) to generate the reduced-order solution for the case 
V_{inlet} = 0.8 [m/s]*sin(2*pi*(0.3) [Hz]*t)   (amp =0.8, freq =0.3)

For comparisons: Full-order simulation takes around 8.5 hours, while ROM solution takes only 4 to 5 minutes. The discrete energy 
is preserved at around 88%. The movie comparisons are provided.
