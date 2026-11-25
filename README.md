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

One of these has to give. A heating-rate scan is the experiment that decides it, and it has not
been done at these temperatures.

## What the experiment did

Supercooled water is hard to study because it freezes. You et al. sidestepped that by starting
from low- and high-density amorphous ice and heating it with infrared laser pulses, then probing
the result with x-ray scattering before ice could form.

Sweeping the laser fluence moved the sample through a range of liquid states. Across that range
they report three things: a crossover from discontinuous to continuous behaviour, broad and slow
structural changes consistent with critical fluctuations, and a rapid heat-capacity increase
peaking at 210 ± 8 K.

That is a coherent story. The peak position, the fluctuation length scale and the slowing down
all point the same way.

## What the reinterpretation says

Pabst & Hassanali ran simulations with MB-pol, a machine-learned potential trained on
high-quality water data, and coupled them to the Tool–Narayanaswamy–Moynihan model of the glass
transition. That model describes how a glassy material's structure lags behind its temperature
when you heat it.

Heating fast puts the sample out of equilibrium. As rotational and translational degrees of
freedom unfreeze, the system absorbs energy at a rate set by the relaxation time, not by any
phase boundary. The result is a peak in apparent heat capacity at roughly the observed
temperature, with no critical point involved.

They add a second, independent argument: their predicted glass-transition temperature sits close
to where electron diffraction sees structural arrest in supercooled water. Two different
observables pointing at the same temperature is suggestive, though not decisive.

## The test that separates them

The two pictures predict different behaviour under a change of heating rate.

For a glass, the endotherm moves. Its position is set by where the relaxation time crosses the
timescale of the measurement, and relaxation times are strongly temperature dependent near the
glass transition. Heat ten times faster and the peak shifts by several kelvin. This is standard
glass phenomenology, and it is why differential scanning calorimetry reports a rate-dependent
glass transition rather than a fixed one.

For a critical point, the peak does not move. The coexistence line sits where the phase diagram
puts it. Changing the rate changes how much of the transition you resolve and how sharp the
feature looks, not where it is.

So: one sample, five or six heating rates spanning a couple of decades, and watch whether the
peak walks.

- If it walks in step with the TNM prediction, the 2026 signal was a glass relaxing, and the
  liquid–liquid critical point remains unobserved.
- If it holds position while the amplitude grows, the Pabst–Hassanali account fails and the
  critical point survives.

Neither group has published that scan. Ultrafast heating makes it harder than a calorimetry
experiment, since each rate needs its own pulse shaping and its own probe timing, but the range
of rates is not the obstacle. The obstacle is that nobody has run it.

## What independent work already constrains

Not everything points the same way, which is why this is a live dispute rather than a settled
one with a lagging minority report.

Kringle, Thornley, Kay and Kimmel (*Science*, 2020,
[doi:10.1126/science.abb7542](https://doi.org/10.1126/science.abb7542)) obtained infrared spectra
of supercooled water films between 135 and 235 K, formed for nanoseconds by ultrafast heating and
cooling. Over that range they found the structure of water to be a **linear combination of a
high-density and a low-density liquid**.

That cuts against the pure glass reading. A two-component description of the structure is what
you expect if two liquid states coexist, and it is not what a single relaxing glass gives you.
It also makes the Pabst–Hassanali result harder to dismiss in the other direction: they reproduce
a heat-capacity peak with a one-relaxation-time model, but that model has to coexist with
Kringle's two-component structural data.

So the ledger is genuinely split. An experiment sees a heat-capacity divergence. A simulation
reproduces it without criticality. A separate experiment sees structural evidence for two liquid
states. That is a disagreement worth watching, not a case where one side has already lost. The
rate scan is still the cleanest way to break the tie, because it tests the mechanism directly
rather than inferring it from structure or thermodynamics alone.

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
