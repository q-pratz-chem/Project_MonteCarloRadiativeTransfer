# Project: Monte Carlo Radiative Transfer

My individual project on writing python code to simulate how the radiation from a star propagates 
through a surrounding gaseous interstellar medium along with the written report from the scientific
investigation from the analysis done using the written code.

“Radiative transfer" is the collective term for a large, complex set of processes that govern how 
radiation propagates through different media. Accurate models of radiative transfer are important 
in many areas of physics, though they plays a uniquely central role in astrophysics. Virtually 
everything we know about the universe empirically is derived from measurements of electromagnetic 
radiation that propagated through space from some distant astronomical source to our telescopes.

One of the major challenges faced by numerical codes that simulate radiative transfer is
that it is prohibitively expensive to track the propagation of individual photons. A common
method for dealing with this is to use Monte Carlo techniques to model the probabilistic
behavior of photons.

Setup of problem:
- Assume that the radiation source (a star) can be represented as a point source
in the middle of your simulation domain, and consider motion only in a 2D plane.

- Photons are assumed to travel radially outward from the star through a uniform
gaseous medium until they interact with a gas molecule, resulting in either a
scattering or an absorption event.

- Assume that all photons are exactly alike – that is, you don’t need to assume
different behavior for photons of different frequencies, just assume all photons
experience the same absorption and scattering probabilities when interacting
with the gas.


