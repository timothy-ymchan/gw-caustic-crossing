## 3rd June 2023

### Further work
1. Try to work out why the velocity addition formula look the way it is (like in Oguri etc.)
2. Remember that in reality such macro+single micro senario is rare, so actually this might need some justification
3. You might also want to justify the how far the macro-micro lens are separated in order for this treatment to work in wave optics (or it simply does not work and directly treating two lenses with wave optics is necessary.) (Actually with the code of Mark Cheung you might want to try to compare the analytical solution with the approximate one).

### Progress:
Worked out the criteria for the applicability of the formalism.

**Results:**
1. For macrolens similar to Sgr A*, the formalism is applicable so long as the Einstein radius of the microlens is smaller than 1 arcsec (which is always true because those have $\theta_E\sim$ 1mas).
2. The applicability depends on the magnification. In general the $\theta_m$ needs to be smaller if the magnification increase.
3. There is a hidden problem with the formalism when applied to moving lenses. In particular the time scale of which $\mu_t$ changes should be much less then the Einstein crossing time. Otherwise, the background potential would have changed much quicker than the crossing. This depends on the third derivative information of the macrolens, though. **An estimation about the validity of this has not been done yet.**


### Project Plan:
What I have right now:
1. Caustic crossing lensing where there is an external shear field.
2. The external shear field makes the caustic crossing easier to occur, allowing us to look further in space.
3.  We now know how to modify the waveform.

Questions:
1.  Is this formalism appropriate, compared to the field of micro lenses? (i.e. in a practical sense)
2.  Wavelength compared to the separation of the lenses, is this justified? Or is it better to consider it as a system of two lenses of different masses?

Plan:
1.  Work out the criteria for which the macro-micro lens model is applicable. (I.e. how short the wavelength must be)
2.  From your previous works you have a set of criteria for detection in high frequency, monochromatic wave regime.
3.  Give DECIGO & LISA a try according to the results in (1)
4.  Do the waveform modelling and mismatch computation to provide another confirmation of the criteria in (2)
5.  Rate estimation

### The set of criteria of detection so far
1. A time delay estimate $\Delta t_d\gtrsim 1\text{ms}$