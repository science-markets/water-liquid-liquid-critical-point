# Water's second critical point: what the 2026 experiment shows, and what it doesn't

In March 2026 a group led by Anders Nilsson, Peter Poole and Katrin Amann-Winkel published
evidence for a liquid–liquid critical point in supercooled water, at **210 ± 8 K** and about
**1 kbar**. It was covered as the end of a thirty-year hunt. By September a preprint argued the
same measurement follows from ordinary glass physics, with no phase transition at all.

Both papers are careful. Both are consistent with the same x-ray data. The disagreement is about
what that data means, and it is not resolved.

- Experiment: You et al., *Science* **391**, 1387–1391 (2026), [doi:10.1126/science.aec0018](https://doi.org/10.1126/science.aec0018)
- Reinterpretation: Pabst & Hassanali, [arXiv:2609.26442](https://arxiv.org/abs/2609.26442) (22 Sep 2026)

## The short version

The experiment measured a sharp rise in heat capacity while heating amorphous ice fast enough to
outrun crystallization. A diverging heat capacity is the signature of a critical point. The
preprint reproduces the same rise in simulation by treating the sample as a glass relaxing toward
equilibrium, which also produces a sharp feature at a similar temperature.

One of these has to give. The preprint's own argument for how to settle it is a change of heating
rate, and the experiment that would do that cleanly has not been run.

## What the experiment did

Supercooled water is hard to study because it freezes. You et al. sidestepped that by starting
from high- and low-density amorphous ice and heating it with infrared laser pulses, then probing
the result with x-ray scattering before ice could form.

Sweeping the laser fluence moved the sample through a range of liquid states. Across that range
they report three things: a crossover from discontinuous to continuous behaviour, broad and slow
structural changes consistent with critical fluctuations, and a rapid heat-capacity increase that
they locate at 210 ± 8 K. The abstract's own verb is "suggest" — they write that the results
suggest the experiments probed the vicinity of a critical point, not that they proved one.

## What the reinterpretation says

Pabst & Hassanali ran simulations with MB-pol, a machine-learned potential trained on
high-quality water data, and coupled them to the Tool–Narayanaswamy–Moynihan model of the glass
transition. That model describes how a glassy material's structure lags behind its temperature
when you heat it.

Heating fast puts the sample out of equilibrium. As rotational and translational degrees of
freedom unfreeze, the system absorbs energy at a rate set by the relaxation time, not by any
phase boundary. The result is a peak in apparent heat capacity at roughly the observed
temperature, with no critical point involved.

Two things in the paper make it more than a hand-wave. First, they fitted the TNM parameters at
one heating rate and then predicted the heat-capacity trace at the other with no adjustable
parameters; the prediction matched. Second, their predicted glass-transition temperature sits
close to where electron diffraction sees structural arrest in supercooled water, from a
different group and a different observable.

## The test that separates them

The two pictures predict different behaviour under a change of heating rate.

For a glass, the endotherm moves. Its position is set by where the relaxation time crosses the
timescale of the measurement, and relaxation times are strongly temperature dependent near the
glass transition. Heat faster and the peak shifts up. This is standard glass phenomenology, and
it is why differential scanning calorimetry reports a rate-dependent glass transition rather than
a fixed one.

For a critical point, the peak does not move. The coexistence line sits where the phase diagram
puts it. Changing the rate changes how much of the transition you resolve and how sharp the
feature looks, not where it is.

This is the preprint's argument, not mine. They show the step shifting upward as they raise the
heating rate from 4.16 to 13 K/ns, and they note that the experimental heating rate itself varies
with laser power.

Which is exactly why the existing experiment cannot settle it. In a fluence sweep, rate and
temperature rise are coupled: turning up the laser moves both at once. Separating them needs the
temperature jump held fixed while the pulse duration changes, so the peak either walks or does
not. Nobody has published that. The preprint is explicit that this is a prediction its model
makes and that the experiment to test it is future work.

## What their deposited data says

You et al. deposited the numbers behind their figure 3: laser fluence against the temperature they
estimate it reached. Seven points, 3.07 to 15.53 J/cm²
([doi:10.5061/dryad.pc866t23j](https://doi.org/10.5061/dryad.pc866t23j)). The heating rate is the
temperature jump divided by the time taken to deposit the energy, and the deposit gives the first
half of that fraction but not the second. So it can be read but not computed outright.

Two things come out of it.

First, fluence and temperature are not proportional. Fluence rises by a factor of **5.1** across
the sweep. The temperature goes from about 175 K to about 210 K, which measured as a jump above
the 135 K starting point is a factor of **1.9**. Four of the five points above 5 J/cm² sit within
3.8 K of one another — the fifth, at 15.5 J/cm², is 4.6 K above the highest of them. Their fit
curve moves about half a kelvin when fluence doubles from 9 to 18 J/cm². Whatever else the sweep
is, it is not a hidden rate scan.

Second, the sweep does not cross the rate interval the preprint argues about. Across the region
where the heat capacity climbs — 5.13 to 15.53 J/cm², heat capacity from about 3.6 to 10 J/(g K) —
the temperature jump goes from 69.6 to 75.1 K. If the deposition time is anywhere near constant,
that is a rate change of about **8%** while the signal roughly triples. Pabst & Hassanali's
decisive comparison is 4.16 against 13 K/ns, a factor of 3.1.

Which is a strange result to sit with. The preprint needs the rate to move a factor of three to
shift its endotherm visibly. The experiment varies that same quantity by under a tenth over the
interval where the heat capacity triples. I do not know what reconciles those, and neither paper
raises it. The most likely answer is that the deposition time is not constant across the sweep,
which would make my 8% figure wrong — but the deposit does not say, and I could not get the
supplement.

The limits: these are deposited estimates, not raw scattering, and I have not propagated the
per-point temperature uncertainty. The heat capacities above are not in the deposit either. I
computed them with the conversion Pabst & Hassanali spell out in their methods — absorbed fraction
17.1% from an absorption coefficient of 50 cm⁻¹, 35.3 µm effective thickness, 0.94 g/cm³ — the same
constants they used to put both datasets on one axis. Change those and the tripling changes with
them, though not by much: the uncertainty in the absorbed fraction enters the heat capacity
linearly.

## The authors' own caveat, which cuts both ways

Pabst & Hassanali end by questioning whether heating experiments can ever answer this. Their
words: it is "questionable whether such heating experiments can ever detect equilibrium two-state
fluctuations underlying a possible liquid-liquid transition, or whether nonequilibrium dynamics
such as those revealed here will inevitably mask them." They suggest ultrafast *cooling* as the
more promising route, since the anomalous heat capacity has been seen that way.

Take that seriously. It is a reason the dispute may not be settled by any heating experiment, and
it is the authors conceding a limit on their own framing as much as on the original one.

## What independent work constrains

Not everything points the same way, which is why this is a live dispute rather than a settled one
with a lagging minority report.

Kringle, Thornley, Kay and Kimmel (*Science*, 2020,
[doi:10.1126/science.abb7542](https://doi.org/10.1126/science.abb7542)) obtained infrared spectra
of supercooled water films at temperatures from 135 to 245 K, formed for nanoseconds by ultrafast
heating and cooling. Over that range the structure of water was a **linear combination of a
high-density and a low-density liquid**. That is the main structural evidence that two liquid
states exist.

Now the honest complication, and the preprint states it plainly: in water, the glass transition
is accompanied by a pronounced structural transformation at the same temperature. So a two-state
structural description does not by itself distinguish "two coexisting liquids" from "a glass
unfreezing into a liquid." Structure and mobility change together, and their shared temperature
dependence cannot tell you which one is doing the work.

So the ledger is split in a specific way. An experiment sees a heat-capacity divergence. A
simulation reproduces it without criticality and fits the structure too. The structural data that
looked like proof of two liquids does not separate the two pictures. What separates them is rate,
which is why the rate scan keeps coming back.

## What this page is not

This page is an explainer. It is not research, it does not settle anything, and it is not part of
how any market resolves.

Nothing here has anything to do with settlement or pricing. science.markets runs a market on this
question, and this page is not a resolution source, not an evidence submission, and not a
statement of what the market will resolve to. Where this page and a source disagree, the source
is right.

I do have an interest: science.markets lists [the market in
question](https://science.markets/markets/water-liquid-liquid-critical-point/?ref=gh). Treat that
as a reason to check the two papers rather than trust the prose above. Both are open: the
preprint is on arXiv, and the *Science* paper's abstract and figures are readable without a
subscription.

Corrections are welcome as issues. If you run the rate scan, or know of one that exists, that is
the thing worth telling me.
