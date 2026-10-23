# Keep cool-water refuges from mixing away

Research reviewed October 23, 2026. AI-assisted family background research. This is the strongest overall candidate in this comparison for a conditional physical pilot, not a selected or validated project.


### Plain problem and actual environmental action

A small cold tributary can enter a warm river and immediately mix away, leaving little accessible cool water for temperature-sensitive wildlife. The proposed physical intervention is a small, adjustable flow deflector immediately upstream of the confluence. It redirects some warm main-channel flow away from the cool inflow so that more cool water remains connected to the river. **It does not manufacture cold water, extract new groundwater, or increase the tributary's supply.**

The environmental improvement to measure is a larger connected volume of cooler water, sustained for longer, at the same cold-water and main-channel inputs. A colder but smaller pocket, a blocked-off pool, or an improved prediction is not sufficient.

### Primary need, existing restoration, and novelty limits

Cold-water refuges are an established management need. The Lower Columbia Estuary Partnership's 2015–2018 investigation examined tributary cold-water sources and modeled flow-diversion structures to enhance their plumes. Its project account identifies a historical 57-mile gap in suitable refuges and explains that some smaller tributary plumes dilute immediately. This is a documented regional example, not a claim that the same gap is unchanged today. [Primary project report, 2018](https://www.estuarypartnership.org/sites/default/files/resource_files/LCEP%20Lower%20Columbia%20Thermal%20Refuge%20Report%20FINAL_small.pdf); [implementing partnership's project account](https://www.estuarypartnership.org/cold-water-refuges).

The underlying intervention is already known. Kurylyk and colleagues explicitly proposed controlling advective mixing to augment tributary thermal anomalies; the paper appeared online in 2014 and in the 2015 journal volume. A 2025 practitioner/research synthesis reports actual confluence restoration using channel narrowing, rocks, cover and deflectors. Do not claim invention of a thermal deflector or the first engineered river refuge. [Kurylyk et al., primary research/concepts](https://doi.org/10.1002/eco.1566); [Quilbé et al., 2025, restoration cases and limitations](https://doi.org/10.1002/rra.4462).

Professional commercial practice already covers this territory. Natural Systems Design describes reducing warm-water mixing and designing thermal-deflector/complex-edge structures in the Pacific Northwest. A 2026 patent also describes an actively temperature-controlled aquatic refugium, although its heating/cooling apparatus differs from the natural-inflow deflector here. A patent is prior art, not evidence of ecological effectiveness or a determination of freedom to operate. [Restoration provider's account](https://naturaldes.com/protecting-thermal-refuges-for-coldwater-fish-in-the-pnw/); [US12653165B2, published 16 June 2026](https://patents.google.com/patent/US12653165B2/en).

ML prediction is not new either: Hani and colleagues modeled hourly potential refuge area at two confluences using supervised models. Their study supports nonlinear responses to river conditions, but does not establish that a learned controller will outperform a well-designed passive structure. Its data are available on request rather than a verified immediately downloadable action/outcome training set. [Primary ML study, 2023](https://doi.org/10.1002/rra.4191).

**Narrow proposed contribution:** physically demonstrate whether a learned choice of deflector angle maintains more connected cool-water volume across previously unused flow/temperature sequences than a competent fixed structure and tuned conventional controls, without extra cold water, restricted flushing or extra backwater. That contribution remains unverified. If one passive angle performs best across the realistic conditions, use that engineering result and drop the claimed need for ML.

### Simple hardware and a realistic indoor core

Build a clear freshwater channel roughly 0.8–1.2 m long, with a small side inlet representing the cool tributary, a fixed near-bank refuge region and an overflow that sets water depth. Use one main-channel pump, a separately metered cool-inflow pump, an above-water servo/hinge for one deflector, and replaceable printed inlet/bed inserts. No moving vehicle, underwater navigation or field installation is required.

Start with a fixed, non-eroding bed. A sand-bed extension is not necessary; otherwise morphology and sediment accounting could consume the schedule. One adjustable angle is enough initially. Use five mechanically reproducible angle settings, with identical deflector material, maximum footprint and access gap for all controllers.

The apparatus needs two inlet temperatures, not summer weather. A warm reservoir and an insulated cool reservoir emulate the river and its existing tributary. Ordinary listed aquarium heating equipment, room-temperature water and sealed cool packs can establish these inlet conditions under the approved protocol. Cooling the experimental feed is **boundary-condition preparation**, not a proposed field refrigeration system. Record that preparation and electricity rather than implying the bench obtains cooling without a source.

A main recirculation loop can conserve water, but mixed return water will change the warm reservoir temperature. Log the actual inlet temperatures and volumes continuously, control or reset them, and account for the added cool-water volume and corresponding reservoir overflow. Do not compare a fresh cool reservoir with a progressively warmed one. Avoid two loops that exchange unaccounted water. Confirm actual pump flow at the installed head and deflector settings; nominal pump ratings are inadequate.

Use enough flow and depth that the experiment is not simply two unmoving layers in a shallow dish. Record discharge, channel cross-section, mean velocity, water depth, temperature contrast and relevant Reynolds/Froude or density-flow similarity limits. A small flume cannot match every field parameter simultaneously. A mentor with fluid-mechanics experience should review this before claiming transfer to a river.

### Temperature, connected volume and flushing measurements

Reserve approximately 27 temperature positions within a predeclared three-dimensional refuge region, including near-bed, middle and upper depths, plus main inlet, cool inlet and mixed outlet probes. The array must actually cover the plume; adjust the physical grid during the pilot and freeze it before confirmation. A surface photograph or a single bottom sensor cannot establish volume.

One affordable manufacturer anchor is the DFRobot waterproof DS18B20 family at $6.90 each, with the DFR0198 listing a 10–49 price of $6.20 and nominal accuracy of ±0.5°C. Adafruit lists a comparable probe at $9.95, or $8.96 for 10+. These are price/specification anchors, not a guarantee of delivered cost or measurement performance. [DFRobot probe](https://www.dfrobot.com/index.php?path=36_64&product_id=689&route=product/product); [small encapsulated alternative](https://www.dfrobot.com/product-2481.html); [Adafruit probe](https://www.adafruit.com/product/381).

Calibrate all probes together in well-mixed baths spanning the actual range and check a reference thermometer with a stated uncertainty. For example, Hanna lists the HI98501 at ±0.2°C over the relevant range; its specification does not certify the whole array. Measure each probe's lag as well as bias. A 0.0625°C digital step or a 750 ms conversion time is not 0.0625°C accuracy or the waterproof package's physical response time. Use control intervals slower than the verified thermal response. [Reference thermometer specification](https://hannainst.com/hi98501-checktemp-digital-thermometer.html).

Primary quantities:

- **Sensor-resolved connected cool-volume estimate**, in litres, and its time integral in litre-minutes. A provisional physical criterion is at least 2°C cooler than the contemporaneous main inlet; report sensitivity to other temperature contrasts. This is an engineering comparison threshold, not a universal fish-survival limit.
- **Volume–temperature distribution and continuous temperature-deficit integral**, such as litre-degree-minutes, so the result cannot conceal cooling fewer litres more strongly. Report inlet and outlet heat transport too.
- **Physical connection to the main channel:** continuous open-water path, measured minimum entrance width/depth, and water exchange through it. No mapping from miniature clearance to fish body size is assumed.
- **Flushing/retention behavior:** an approved dilute dye pulse and fixed-camera measurements can compare tracer arrival and washout at the entrance, inner pocket and outlet. Calibrate color response and use the same optical geometry. Tracer transport is a separate check of physical exchange, not evidence of fish movement or adequate oxygen.
- **Backwater, channel throughput and actuation:** water-level rise, actual main flow, cold flow, actuator movement and failure rate. A design that makes a large cold pocket by obstructing the river or sealing off the pocket fails.

Interpolate only within the measured region and report sensitivity to probe spacing, threshold uncertainty and interpolation. For steady confirmation states, reposition the array in additional repeat runs to obtain denser profiles and test whether the coarse grid ranks designs correctly. Quantify probe/rack obstruction with changed rack positions and sparse-probe/tracer checks. Do not present interpolated cells as independent observations. If sensor lag, grid gaps or physical interference prevent a reliable volume estimate, reduce the claim to measured area/depth rather than inventing volume—or reject the project if that no longer meets the selected criteria.

### Fixed cold-water budget and heat balance

Match the **measured** main-inlet flow profile, cool-inlet flow profile, inlet temperature histories, initial water state, depth, run duration and footprint between controllers. In addition to total cool litres, compare the cumulative supplied thermal contrast:

`cold-input thermal budget = ρ cp ∫ Qcold(t) [Tmain(t) − Tcold(t)] dt`.

This does not mean coldness is created or a complete ecological value is assigned to joules. It prevents a controller benefiting from more or colder feed. Predeclare tolerances after calibration and before confirmation; repeat invalid boundary-condition runs using a consistent rule rather than selecting attractive traces.

For the flume control volume, check the approximate heat balance:

`change in stored heat = inlet heat transport − outlet heat transport + heat exchanged with surroundings`.

Measure inlet/outlet temperatures, discharge and storage; estimate heat exchange using appropriate baseline runs with the same flow, room conditions and duration. If the outlet is not mixed, a single outlet probe is insufficient: use a downstream mixing collector or a verified flow-weighted measurement. Keep pumps/heaters outside the flume control volume so their effect is reflected in measured inlet temperatures, or explicitly include their contributions. Report reservoir drift and unexplained residuals. A deflector redistributes an existing cool input; it cannot lower the whole-river mean temperature beyond the available heat budget.

### ML that changes the intervention, with serious baselines

Collect original randomized action-response episodes over realistic main/cool flow ratios, inlet temperature differences and a limited depth range. Inputs can include measured flows, inlet temperatures, current deflector angle and a short history from a few local probes. Output is predicted connected cool volume and exchange/backwater constraints for each possible next angle. A small Gaussian-process or regularized tree model is more appropriate than a deep network or model-free reinforcement learning on a few dozen runs.

The model selects a physical angle; the servo makes the change. Prediction accuracy is secondary to the measured improvement after the action. Training labels come from the independently processed temperature grid and measurements, not from the controller judging its own success. Monitoring archives can set plausible ranges but do not supply causal labels for this apparatus.

Compare four approaches using the same apparatus and development budget:

1. The best **passive fixed deflector** chosen across the development regimes, plus an unobstructed reference used to establish the basic physical effect.
2. A tuned **flow/temperature rule controller**, allowed a lookup table, hysteresis and the same measured signals.
3. A simple **physics/gray-box controller**, fitted to development data using heat balance and low-order exchange/advection behavior, with the same angle and movement constraints.
4. The learned action-outcome controller.

ML might help where changes in flow ratio, density contrast and transport delay produce context-dependent best angles. Those interactions must actually appear. A neural-network label or better forecast does not establish advantage over a tuned rule. The controller must also outperform a robust passive design enough to justify its cost, energy and maintenance; otherwise passive restoration is preferable.

### Ten-day pilot and independent confirmation

**All experimental dates below begin only after any required SRC approval.** Literature, planning and the student's own proposal preparation can proceed beforehand. The November 13 submission deadline is not approval. Disclose the actual fabrication, moving hardware, water/electricity, heating equipment and tracer materials. Current family rules notes are [here](../../research/rules-and-timeline.md).

Pilot days 1–3: assemble the simplest two-temperature channel, calibrate inlet flow and probe bias/lag, and demonstrate a stable confluence plume without a controller. Days 4–6: test the volume grid, input matching, heat budget and exchange measurement. Days 7–10: compare roughly three angle settings under four inlet regimes with two independently reset repetitions, approximately 24 short episodes. The pilot's purpose is to find a genuine angle-by-condition tradeoff and a resolvable physical outcome, not to train impressive-looking AI.

Proceed only if the following are satisfied:

- Cold-volume estimates and repeated boundary conditions distinguish the treatments beyond their uncertainty; sensor/rack effects do not determine the answer.
- The best angle changes meaningfully across realistic regimes, and the larger cool region remains physically connected and flushing.
- A simple flow-ratio/temperature rule is not already sufficient. If one passive angle works well throughout, stop the ML version.
- There is enough operating margin to avoid unacceptable backwater, entrance closure or a motion-created artificial effect.

After the pilot, allow about 40–60 development episodes, grouped by whole day/initial condition for training/validation splits. Freeze all four controllers and measurement processing before final testing. A feasible confirmation allocation is **four controllers × three unfamiliar inlet time sequences × three independently reset day blocks = 36 runs**. Increase replication if pilot variability requires it; three blocks are a practical floor, not a power calculation. All repeated sensor samples within one run are one correlated trajectory. Randomize method order within blocks and reset thermal conditions between runs. Hold out complete time sequences rather than random timestamps. A changed inlet orientation or bed insert is a useful extra transfer challenge only if core confirmation is already complete.

Judge success by connected cool litre-minutes at matched thermal input with no deterioration beyond declared exchange/backwater limits. A selection target could be a practically useful improvement of about 20% over the strongest conventional controller, provided total uncertainty is substantially smaller. This is a go/no-go target, not a predicted result or a universal ecological effect size. Report failures and the full tradeoff; do not select the single temperature threshold that makes ML win.

### All-in planning budget

| Item | Allowance |
| --- | ---: |
| Clear channel, side inlet and collection/overflow pieces | $125 |
| Two pumps, tubing, flow adjustment and plumbing | $145 |
| Reservoirs, cooler and insulation | $70 |
| Approximately 30 waterproof temperature probes | $220 |
| Reference thermometer/calibration supplies | $70 |
| Controller, sensor-bus wiring, logging and low-voltage power | $60 |
| Deflector actuator, position check and linkage | $45 |
| Listed thermal-boundary equipment and cool-pack allowance | $50 |
| Flow/level calibration and tracer/collection supplies | $50 |
| Printed parts, repeated-run spares and consumables | $35 |
| Individual fair entry fee | $40 |
| Basic protection and dry display allowance | $35 |
| Tax, shipping and contingency | $120 |
| **Total** | **$1,065** |

Existing printer, cutter and computer are excluded. The base allowance assumes access to a phone camera for tracer imaging; if needed, add a $40 USB-camera allowance, for a $1,105 total. Except manufacturer anchors, these are procurement allowances, not delivered quotes. Thirty Adafruit probes at the stated quantity price would add about $50 relative to the sensor allocation, still below $1,200. Verify actual pump performance, reference-thermometer price and availability before ordering. The remaining headroom depends on the camera and sensor choices; it is for uncertainty, not a second experiment. Do not delete calibration or repeat runs to buy robotics.

### Season, access, rules and transfer limits

The core is indoors, freshwater and nonbiological; it needs neither summer field water nor fish/coral access. No natural stream alteration is assumed. Actual field deployment requires professional river design, landowner/agency permissions, flood/debris review and ecological assessment. It cannot be inferred from the bench prototype.

With approval in late November, budget approximately ten weeks: first two for the pilot, three for development, one for frozen-control selection, three for confirmation and one for failures/analysis. Finish physical work by late January/early February. If approval, fabrication or calibration slips materially, shorten the question rather than dropping independent confirmation. About 8–12 student hours/week is plausible, but troubleshooting and thermal resets are real labor costs.

The fair display must be dry; videos and the safe dry mechanism can communicate the experiment. The local rules prohibit displayed water and have prototype-size restrictions. The mentor's contribution and any AI assistance must be documented; these notes are not a submission to copy. [Official dates](https://science-fair.org/students-parents/important-dates/); [local SRC](https://science-fair.org/rules-and-registration/src/); [display rules](https://science-fair.org/students-parents/project-display-rules/).

This can show an actual reduced thermal-pressure condition in a contained model. It does **not** show fish occupancy, survival, migration, adequate oxygen, refuge capacity for a species or population recovery. A tiny cold plume might remain ecologically unsuitable. Flow-scaled dimensions, turbulence, density effects, bed mobility, debris and seasonal cold-source reliability differ in a river. Preserving some thermal gradients and access to warmer feeding areas may also matter. The student should describe a thermal-habitat engineering prototype rather than a proved fish rescue device.

**Decision:** strongest new inland direction found in this pass, conditional on the pilot. Environmental purpose is direct habitat protection/restoration. Physical feasibility is good within the cap; ML advantage and competition-level originality are unproven. The strongest possible result is a robust improvement against serious conventional engineering, with transparent limits and a reusable physical action/outcome dataset.


[Comparison and selection](../../README.md) · [Shared rules](../../research/rules-and-timeline.md) · [Validation requirements](../../research/validation-and-selection.md)
