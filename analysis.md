
**Analysis:**
Your analysis should include an examination of these key quantities at a minimum:
1. The fraction of emitted photons that are absorbed (and the corresponding fraction that escape the max radius).
2. The average number of scatterings for escaping photons and for absorbed photons, and 
the fraction of photons that experience zero scattering events.

**Test the effects of the following:**   
(i) Varying the optical depth  

(ii) Varying the albedo  

(iii) Varying the number of rays and examining the convergence of the results

(iv) Extend your calculation to 3D, assuming spherical symmetry around the star.
(Note: because the differential surface element in spherical coordinates dΩ = sin(θ)dθdφ 
depends on the polar angle θ, its probability distribution is not uniform. In order 
to draw uniformly distributed points on a sphere, you should define a random variable z 
that is uniform in $\[0.0,1.0)$ and use the transformation method find a function θ(z) 
that returns the correct probability distribution p(θ) = sin(θ)/2.)  

(v) Make the optical depth a function of the distance from the star, rather than keep-
ing it constant throughout the simulation domain. (This is essentially equivalent
to assuming that the number density and/or interaction cross section of the gas
particles is a function of the distance from the star.)
