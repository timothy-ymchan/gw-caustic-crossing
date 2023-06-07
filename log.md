## 7th June 2023

### Further work
1. Plot the new time delay with the source term (which you originally ignored in the previous computation.)
2. Tried to parameterize the time delay curve using the reduced variables (which should be easy)
3. Read the degeneracy paper (https://arxiv.org/abs/2104.07055)
4. Write the waveform and try to look at it
### Progress
1. Worked out from first principle the time delay of the PML including the source part $\psi(\vec \beta)$

### Goal of the day
1. To work out the time delay of point mass lens with a source term
2. Suppose source position $\beta$ is changing with an effective source velocity $\dot \beta$, compute the time delay curve (possibly analytically)

### Some thought about degeneracies
1. In GW observation (best case), and assuming the signal is monochromatic (for simplicity), the signal would looks like $\sqrt{\mu(t)}A_0\cos\left[2\pi f_0(t-\Delta t_d(t))\right]$.
2. When $t\to \infty$, we should be able to find $A_0$ and $f_0$ because $\sqrt{\mu(t)}\to 1$ and $\Delta t_d\approx \text{const}$.
3. The time scale of $\sqrt{\mu}$ or $\Delta t_d$ change will give the Einstein crossing time $t_E$ and depending on the exact form of $\Delta t_d$ we might be able to work out also $u_\text{min}$ using information around the peak of the timing curve.
4. Now onto the degeneracies, recall that $\theta_E=\sqrt{4M D_{LS}/D_L D_S}$ in geometric units, and that $t_E=D_L \theta_E/v_\perp$, $u_\text{min}=\beta_\text{min}/\theta_E$, and $\dot \beta=v_\perp/D_L$. Note that we cannot get $\theta_E$ from the timing curve/magnification curve alone, because we don't know the source position.
5. Furthermore, we can write $D_L=4MD_{LS}/\theta_E^2D_S$ and if local universe $D_{LS}=D_S-D_L$ so we if we write $D_S\to kD_S$, $v_\perp\to k v_\perp$, $D_L\to kD_L$, $M\to kM$. Of course there are additional degeneracies, we have $D_L,D_S,M,v_\perp,\beta_\text{min}$ as free lens parameters, but we only have three constraints $u_\text{min}, t_E$, and $\dot \beta$. 
6. Suppose wave optics can resolve $M$ (or $\theta_E$), then we are left with one free parameters.
7. If it is not monochromatic, we might also be able to infer the time delay $\Delta t_d$ between the images, this might give us full recovery of lensing information.

## 5th June 2023

### Further work
1. Try to think about (3) in progress a little more
2. Try to search for papers in GW side that actually looked at such lensing cases.

### Progress
1. The derivation for the velocity formula is essentially the same as what I have derived before, so the complication is not there.
2. The paper by Gravitational Microlensing at Large Optical Depth by Paczynski is well-written and introduces the formalism of background shear + multiple lenses. In fact, that have also been investigated by the gravitaitonal lensing community, just without the caustic crossing part.
3. I suspect that the modification of the lens velocity is due to the fact that the microlens is actually being lensed by the background field. So the position we observe is actually an image position, not really the physical location of the microlens, that might be able to explain why I need to correct that velocity. Otherwise I can't see any reason why the lens velocity have a number of components. 

### Goal of the day
1. Try to work out why the relative velocity is the form it takes in oguri and also in R. Kayser, S. Refsdal and R. Stabell, Astron. Astrophys. 166, 36 (1986)

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