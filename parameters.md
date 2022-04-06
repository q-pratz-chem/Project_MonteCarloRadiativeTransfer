
**Optical depth (distance traveled before interaction):** 
The mean free path of photons through a medium is closely related to the optical depth of the 
medium. The optical depth, denoted by τ, is a dimensionless quantity that tells us the 
likelihood that a photon will be absorbed or scattered while traveling through the medium. A
medium with τ >>1 is called __optically thick__, and a photon traveling through it will
either be quickly absorbed, or it will undergo many scatterings before emerging. A medium
with τ<<1 is called __optically thin__, and a photon is very unlikely to be scattered or
absorbed while traveling through it. A population of photons propagating through a medium 
will interact after traversing different distances s, distributed according to an exponential PDF:

$p(s) = \tau e^{−\tau s}

You will need to use this non-uniform PDF to generate the random distance traveled
by a given photon before its next interaction event. Start by assuming an optical
depth of τ = 1. Given the current direction of travel of a photon, as well as this
distance traveled, we can determine the location of the next interaction event.

**Albedo (scattering vs. absorption probability):**
For each interaction, draw a random number to determine whether the photon is scattered or absorbed. 
The probability of scattering versus absorption can be expressed in terms of the albedo of the
gas particle. A substance with an albedo of 1 will scatter 100% of the photons that
hit it, while a substance with an albedo of 0 will absorb 100% of incident photons.
Start by assuming an albedo of 0.95.

**Scattering angle:** If the particle is scattered instead of absorbed, a new random
scattering direction should be chosen (still assuming motion only in a 2D plane).
•Stopping the simulation: Each photon path should be traced until one of the following criteria
is met: (i) the photon is absorbed, or (ii) the photon reaches a predefined maximum distance 
from the star, beyond which it will be assumed to have “escaped" the gas cloud surrounding the 
star. (Note that the distance units in this scale-free problem are arbitrary). Maximum number
of scattering events are defined as a failsafe in case the simulation takes too long or 
encounters an infinite loop.
  
