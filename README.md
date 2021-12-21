# solving for initial conditions of a 1d diffusion problem given experimental results 

**Experimental data**: Self-diffusion process of 7Li atoms in 6Li metal was monitored (over time) by NMR measurements. At the start, due to previous experimental procedure, the isotopic fraction of 7Li is relatively high close to the metal surface. Then, due to the self-diffusion process, more and more 7Li atoms diffuse towards the metal bulk (which is beyond the NMR detection range, see https://en.wikipedia.org/wiki/Skin_effect for details), thus reducing the measureable 7Li intensity.  

**Objective**: Finding the initial 7Li distribution in the metal (i.e., the I.Cs), that explains the observable results. 

**Methodology**: 1) model the self-diffusion process on a 1d grid (using central differences and forward Euler techniques).
                 2) run black-box optimization process to find the I.Cs of the system that fit best to the experimental data (using scipy.optimize.minimize).

