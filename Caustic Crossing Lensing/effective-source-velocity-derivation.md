# Derivation of the effective source velocity formula
There are a number of ways to derive the formula (See for example, Kayser et. al. (1986)). Here we present a derivation that add up the angles directly.

We recall the following facts about angular diameter distances in a flat cosmology (i.e. $\Omega_k=0$).


**(C1) Addition of angular diameter distances:**

Let $D_2>D_1$ be the angular diameter distances between two points. The angular angular diameter distances between the two points are:
$$D_{12} = D_2 - \frac{1+z_1}{1+z_2} D_1$$
where $z_1,z_2$ are the redshifts of point 1 and 2 respectively.

**(C2) Inversion of angular diameter distances:**
$$
\frac{D_{12}}{D_{21}} = \frac{1+z_1}{1+z_2}
$$

**Main derivation:**

Now we can derive the velocity addition formula. First, by elementary geometry, it is easy to see that,
$$
    d\beta_s = d\ell_S/D_{OS}\\
    d\beta_l = -d\ell_L/D_{OL}\\
    d\beta_o = d\ell_O \left(1/D_{LO} - 1/D_{SO}\right)
$$

where $d\beta_{s/l/o}$ are changes of apparent angular position of the source due to source, lens, and observer movement respectively and $d\ell_{S/L/O}$ are the physical, transverse displacement on observer, lens, and source plane. The angular diameter distances $D_{ij}$ refers to the angular diameter distances from $i$ to $j$. We stated the order from which the angular diameter distances are measured explicitly because $D_{ij}\neq D_{ji}$ if cosmology is introduced. 

We can also relate the time on lens and source plane $dt_{l/s}$ to that measured by the observer $dt_{o,l/s}$,
$$
    dt_{o,s} = (1+z_s) dt_{s}\\
    dt_{o,l} = (1+z_l) dt_{l}
$$
Hence, the combined apparent source angular velocity, measured in observer frame is,
$$
    \dot{\vec\beta} =\frac{1}{1+z_s}   \frac{1}{D_{OS}} \vec v_S - \frac{1}{1+z_l}\frac{1}{D_{OL}} \vec v_L + \left(\frac{1}{D_{LO}} - \frac{1}{D_{SO}}\right) \vec{v}_O
$$
Finally, we can rewrite everything in terms of $D_{LS},D_{OS}$ and $D_{OL}$ using (C1) and (C2).
$$
    \dot{\vec\beta} =\frac{1}{1+z_s}   \frac{1}{D_{S}} \vec v_S - \frac{1}{1+z_l}\frac{1}{D_{L}} \vec v_L + \frac{D_{LS}}{(1+z_l)D_L D_{S}}\vec{v}_O
$$
where we have denote $D_{Oi}$ as $D_i$ for brevity. 

Finally, we can put $\vec v_\text{eff} = D_S \,\dot{\vec{\beta}}$ and obtain the results in Kayser et. al. (1986):

$$
    \dot{\vec v}_\text{eff} =\frac{1}{1+z_s}  \vec v_S - \frac{1}{1+z_l}\frac{D_S}{D_{L}} \vec v_L + \frac{1}{1+z_l}\frac{D_{LS}}{D_L}\vec{v}_O
$$
which is the desired result.