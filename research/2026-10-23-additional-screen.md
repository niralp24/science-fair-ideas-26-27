# Additional research: decisions and exclusions

Research reviewed October 23, 2026. AI-assisted family background notes, not student submission material. This pass screened direct habitat restoration and removal of existing pollution, excluding dredging and projects merely improving a harmful industrial activity.

## Additions from this pass

| Direction | Decision | Why it is distinct and what remains unresolved |
|---|---|---|
| [Oil recovery](../ideas/04-oil-recovery/README.md) | Conditional candidate | Physically recovers existing oil; learned joint depth/speed control must beat passive/PID/lookup methods. Existing skimmers and prior ISEF robots make broad novelty claims untenable. |
| [Native-seed treatment](../ideas/05-native-seed-treatment/README.md) | Conditional candidate | Changes individual seed-coat abrasion, rather than pelleting/watering. Actual healthy seedling yield is measurable, but lot suitability, delayed labels and commercial/patent overlap are significant gates. |
| [Reef rubble](../ideas/06-reef-rubble/README.md) | Higher-risk reserve | Stabilizes a rubble bed while retaining open surfaces; does not retain a transplanted plant plug. Representative substrate, recent prior art, substantial ML value and ecological transfer remain weak. |

None is described as a proven invention, a guaranteed ISEF contender or an approved experiment. New hardware designs must show an independent physical advantage; no environmental benefit follows from a classifier score alone.

## Stream wood restoration: reserve rather than a promoted project


Clearing large wood from streams removes structures that create varied flow, cover and pools. The USGS identifies wood removal among the changes that have impaired Willamette floodplain processes. Restoration is directed at habitat, rather than making logging or a damaging industrial activity more productive. [USGS restoration effectiveness programme, January 2026](https://www.usgs.gov/centers/oregon-water-science-center/science/willamette-focused-investment-partnership-restoration).

## Intervention considered

Use a contained flume to design an open arrangement of small wood pieces that creates more connected low-speed water while retaining an open passage. Hold wood mass and occupied channel footprint fixed; vary at most spacing, orientation and a lower opening. A small learned design model would propose the arrangement, which the student physically builds and tests under changing flow. Constraints would include upstream water-level rise, bank/bed scour, wood movement and obstruction.

An indoor freshwater rig avoids winter field access and fish experiments. A purchasing allowance near $980 is plausible: channel/trays $185, reservoir/plumbing $90, pumps $95, wood/anchors/fabrication $55, controller/drivers $40, depth-grid/point-gauge hardware $85, imaging/lighting $40, collection/weighing $30, repeat bed material $55, protection $35, dry display $30, entry $40, shipping/tax $80 and contingency $120. This is a screening budget, not a validated procurement plan. It does not purchase a scientific three-dimensional velocity instrument.

## Why the prior art is a serious obstacle

- Follett and colleagues already used 584 flume experiments to develop a physics model for backwater around wood jams. The physical habitat/flood-risk tradeoff and wood packing are established engineering questions. [Primary 2020 paper](https://doi.org/10.1029/2020GL089346).
- Müller and colleagues already studied how lower gaps and internal wood arrangements change jets and flow. Their work identifies possible scour effects as well as changed flow patterns. [Primary 2022 paper](https://doi.org/10.1029/2022WR032111).
- A 2025 journal study already varies porous-logjam placement/porosity and develops predictive scour formulas. [Primary paper and publication history](https://doi.org/10.1061/JHEND8.HYENG-13983); [public author manuscript](https://par.nsf.gov/servlets/purl/10579751).
- RETwin already combines reduced-order hydraulic modelling and ML for river habitat prediction/optimization. Its journal year is 2026 despite the 2025 DOI. This is broader habitat optimization, not proof that it solves the particular student rig, but it prevents claiming ML habitat optimization itself as new. [University-hosted author article](https://aaltodoc.aalto.fi/server/api/core/bitstreams/dee89477-1fb7-4e42-b8f4-e0a0a636afb9/content).
- Commercial engineered wood structures have a long history. Forest Concepts' December 2001 technical paper already describes volunteer-installable engineered woody debris. Its existence is commercial prior art, not independent efficacy validation. [Manufacturer's historical technical paper](https://forestconcepts.com/media/Pubs/Pub.Dooley.2001.TechnicalBackgroundEngineeredLog.pdf).

A 2026 long-term field experiment also shows that wood restoration can require maintenance and adaptation over years. A few weeks in a model channel cannot demonstrate those long-term habitat responses. [Primary field study](https://www.frontiersin.org/journals/ecology-and-evolution/articles/10.3389/fevo.2026.1779893/full).

## Measurement and ML weaknesses

A depth map plus overhead surface-tracer motion does not measure the three-dimensional volume of slow water around the wood. The honest affordable endpoint would be a surface-defined low-speed wetted area with measured depth profiles, or a declared area/depth index. Calling this fish refuge capacity or a complete low-velocity volume would be unsupported. A more complete claim requires validated velocity measurements at depth, changing cost and effort.

The strongest simple opponents are the existing hydraulic/scour models, a well-designed conventional wood arrangement and equal-budget factorial/quadratic response-surface optimization. With only two or three parameters, those methods may be sufficient. A Gaussian process is not necessary merely because the response is nonlinear. Showing that some wood slows water would be a demonstration, not a strong new engineering contribution.

For any later pilot, independently reset beds and collect all exported sediment; a benefit cannot be declared by moving erosion to a different bank or downstream. Record all wood failures and throughput. Do not make fish-survival claims or place materials in a real stream on the strength of a miniature flume. Field work would require professional design and applicable permissions.

## Decision

**Reserve only; not promoted to the new idea folders.** The environmental need and basic hardware are sound, but meaningful ML advantage and an affordable, representative habitat endpoint have not been established. Reopen only if a restoration practitioner identifies a specific design failure and the student can measure an independent physical improvement that strong conventional methods cannot already provide. Adding a model to familiar wood-layout experiments is insufficient.


## Abandoned-mine iron: HOLD


**Why the problem matters:** legacy acidic drainage can deposit iron precipitates on stream substrate. [USGS mine-drainage research](https://water.usgs.gov/wrri/grant-details.php?ProjectID=2007PA74B&Type=Annual) documents this mechanism. Treating already-existing abandoned-mine drainage is direct pollution remediation; it is not a proposal to improve active mining.

**Possible mechanism:** use low-cost limestone neutralization followed by iron precipitation and solids capture; adapt contact or cleaning pulses as the limestone becomes coated. This is not new: [USGS's 2003 primary limestone-coating study](https://www.usgs.gov/publications/characterization-limestone-reacted-acid-mine-drainage-a-pulsed-limestone-bed-treatment) describes coating-related failure and a pulsed approach; a [2013 field trial](https://www.usgs.gov/publications/field-trial-a-pulsed-limestone-diversion-well) also experienced plugging and inconsistent performance. Simply adding ML to pH dosing or a cleaning cycle would overlap established control and the family's prior adaptive-treatment ideas.

**Critical measurement problem:** the [Hanna HI721 colorimeter](https://hannainst.com/hi721-iron.html) is $74.99, range 0–5 mg/L, nominal accuracy ±0.04 mg/L plus 2% of reading; [25 reagents cost $14.99](https://hannainst.com/hi721-25-iron-checker-reagents.html). That makes simple iron testing affordable, but **filtered-water iron disappearance is not proof that total iron was captured**. Escaped precipitate can coat a real stream after the water looks clearer. Interferences, dilution, standards, representative influent/effluent sampling and particulate/total-iron recovery need validation. A [manufacturer total-iron method](https://www.hannainst.com/hubfs/product-manuals/MAN802_05_24.pdf) uses acid/persulfate digestion and a heated reactor; that is not covered by the assumed home setup. This does not prove every possible iron assay requires that exact procedure, but it prevents us from pretending a $75 checker closes the total-mass balance.

**Decision: HOLD rather than recommendation.** With a qualified chemistry mentor, validated total-iron method, suitable supervision, disposal pathway and approved synthetic-chemistry plan, a narrowly scoped iron-capture experiment might be affordable. Those resources are not currently established. No actual toxic minewater, mixed heavy metals or unknown microbial cultures should be assumed. Synthetic iron-only tests would establish only that defined chemistry, not comprehensive mine remediation or habitat recovery. A dissolved-iron result alone is inadequate for this family's requirement for real removal.


## Other land routes not promoted


- **Freshwater flushing of salt-damaged wetland soil:** EC measurements are cheap, but salt is shifted into drainwater that must be managed. Existing soil-transport models and timed leaching are strong baselines; no clear non-marginal ML contribution was found for the accessible test. Do not count lower soil salinity alone as a complete environmental solution.
- **Automated native-seed harvest:** seed availability and shattering are real limitations, but the natural harvest season/site access cannot be assumed in this winter timeline. A tray of bought seed cannot validate selective harvest without damaging wild plants or losing genetic diversity.
- **New seed burying robot:** too close to the family's prior seed-restoration proposals and a crowded current field; a new delivery gadget without survival evidence is weak. Native forb emergence can be dominated by site and year rather than apparatus settings ([primary research](https://www.sciencedirect.com/science/article/pii/S1550742422000318)).



## Other cleanup routes not promoted


- Another robot that recognizes plastic and picks it up: overlaps the declined wrack-plastic route and offers no demonstrated useful ML advantage beyond recognition.
- Nurdle/beach-sand separation without a distinct mechanism: meaningful pollution, but existing vacuum/separation devices and the prior beach-removal concept make a generic version crowded. It also needs containment and honest sand/organic-material loss measurements.
- A new oil sorbent recipe: cheap materials alone do not provide the required ML/hardware contribution; it is easy to measure water uptake as if it were oil removal.
- Floating algal-scum harvesting using inert particles: good hydraulic data could be gathered, but that would not establish toxin removal or safe handling of harmful blooms; access and biological assays remain unresolved.
- Reef/coral cleaning with a jet or suction head: forces and artificial-substrate cleaning can be measured, but benefits and tissue injury would remain unvalidated without a specialized facility. It risks recreating a sediment-disturbance project the user has rejected.


[All six project cards](../README.md) · [Rules](rules-and-timeline.md)
