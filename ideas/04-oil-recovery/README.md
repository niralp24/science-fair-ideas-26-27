# Collect spilled oil with less water

Research reviewed October 23, 2026. AI-assisted family background research, not a student-authored fair submission. No prototype, experimental outcome or global novelty claim has been validated.

**Status: conditional marine/inland cleanup candidate. All-in planning total $1,075.**


**Plain problem:** Mechanical skimmers remove floating oil, but waves and changing slick conditions can make them collect unwanted water. A response boat then runs out of storage and must handle a large oily-water mixture. This project removes existing pollution rather than helping extraction operate efficiently. NOAA documents these operational limits and the dependence on thickness and sea state. [NOAA response model](https://gnome.orr.noaa.gov/doc/response.html), [NOAA cleanup explanation](https://response.restoration.noaa.gov/about/media/how-do-oil-spills-out-sea-typically-get-cleaned.html).

**Intervention:** A small stationary rotating drum with an ordinary oleophilic sleeve, scraper and collection trough. A low-voltage actuator changes drum immersion; another motor changes speed. A camera views a wave-height reference and the local slick. The test objective is **more recovered floating oil for a fixed collection-volume and energy allowance**. No autonomous boat, offshore deployment, solvents, custom nanomaterials, gasoline or crude oil is needed.

**What is already solved, and the bounded gap:**

- BSEE's July 2022 report already evaluates 3D-printed drum geometries, thin slicks, speed/submergence settings and vacuum extraction. Printing a drum or optimizing one operating point is not novel. [BSEE Report 1130](https://www.bsee.gov/sites/bsee.gov/files/2023-02/1130ab.pdf).
- Active wave-following skimmer feedback existed decades ago. [EPA's 1980 evaluation](https://nepis.epa.gov/Exe/ZyPURL.cgi?Dockey=9101MIMK.TXT). A servo that follows the water surface is not a new invention.
- Commercial grooved drums already improve pickup geometry. Treat their existence as prior art, not independent evidence of any student prototype's performance. [Elastec](https://www.elastec.com/products/oil-spill-skimmers/accessories/grooved-drum-skimmers/).
- ISEF 2021 ROBO043 already combined an oil-cleanup robot and ML detection. A camera-classifier-cleanup boat is crowded student territory. [Official finalist abstract](https://abstracts.societyforscience.org/Home/FullAbstract?AllAbstracts=True&Category=Any+Category&FairCountry=Any+Country&FairState=Any+State&ProjectId=20502).
- **Narrow possible contribution:** Physically verify that a learned *joint* speed/immersion policy removes more oil before the collection-volume limit than a tuned conventional controller when wave/slick sequences change. This search has not established that nobody has done that exact comparison. A final literature/patent check is essential before claiming novelty.

**Why ML might matter:** The speed maximizing oil pickup can also increase water pickup, and operating choices can depend on previous wetting and changing wave conditions. An empirical multi-output Gaussian-process or small boosted-tree surrogate can learn oil and water collection outcomes from original physical runs, then choose from a limited safe set of speed/depth pairs. Use a short measured history of wave amplitude, visible local slick appearance, motor state and temperature; do not provide hidden ground-truth thickness at deployment. No deep RL or frame-wise train/test splitting.

**Strong baselines:** Best fixed depth/speed from training trials; passive floating head plus a tuned speed lookup table; PID water-following depth plus the same speed lookup; learned joint policy. Give all methods the same drum, motor/collection capacity, development time and sensor inputs where applicable. A passive float that succeeds is a useful result and a reason to reject the ML-led project.

**Contained experiment:** Begin with a single SRC-reviewed, documented, low-volatility food-grade mineral oil or vegetable oil; add a second approved oil only if reset/separation is reliable. This is a defined immiscible-fluid test, not an experiment on toxic, weathered or emulsified crude. Use a reproducible paddle sequence in a secondary containment tray. Independent experimental units are newly dosed, reset runs, not video frames. Plan approximately 30–36 development runs followed by six withheld disturbance sequences × four methods = 24 confirmatory runs, randomized across days. Scope the number from pilot variability and available labor.

**Measurements:** Separate each collected oil/water sample by settling in a calibrated narrow vessel, then read both volumes; independently measure oil density if reporting mass. Include trough drips. Report oil removed/time, oil fraction of collected liquid, oil removed before a fixed total collection volume, and measured electrical energy. Validate the entire separation/readout with blinded known-volume mixtures before comparison. This is **not** a trace dissolved-oil assay or complete mass balance. Emulsion or unresolved layers prevent a valid oil-volume reading. Retain such episodes in the reported denominator as measurement failures, with method and conditions identified; do not discard unfavorable controller outcomes and analyze only separated successes. Systematic method-dependent emulsification defeats this comparison and triggers a stop, rather than selective exclusion; visually disappearing oil is not evidence of removal. Fresh dose minus recovered oil bounds unrecovered material but does not locate it in water versus walls.

**Planning budget, USD:**

| Item | Allowance |
|---|---:|
| Tank and secondary containment | 135 |
| Paddle, drive and bearings | 85 |
| Drum, scraper, sleeve and bearings | 60 |
| Drum motor/encoder | 45 |
| Depth actuator and linkage | 60 |
| MCU, drivers, safe low-voltage supply and wiring | 55 |
| Camera, light and reference | 45 |
| Temperature measurement | 25 |
| Collection and settling vessels | 80 |
| Scale and calibration weights | 45 |
| Fluids, repeated resets and cleaning supplies | 85 |
| Salt for optional final transfer runs | 20 |
| Contained waste handling allowance | 40 |
| PPE | 35 |
| Fair entry | 40 |
| Dry display | 25 |
| Tax/shipping | 75 |
| Contingency | 120 |
| **Total** | **1,075** |

These are planning allowances, not supplier quotations. Confirm fluid disposal locally before procurement; no oily liquid goes down a drain or outdoors. No disposal contractor access is assumed. If an acceptable contained disposal route exceeds the allowance, stop or reduce scale.

**Pros:** Direct removal, judge-readable demonstration, repeatable indoor trials, software chooses physical actions, no live-organism dependence. **Cons:** Extremely crowded topic, modest likely novelty, fiddly cleaning/collection can dominate the schedule. **Mitigation:** Keep the stationary head and a single surface material; invest in accounting and conventional baselines, not robot navigation. **Risks:** Camera appearance changes, emulsification, surface contamination and near-empty slicks can make models unreliable. Restrict the validated envelope and retain failures.

**Go/no-go:** Within two approved pilot weeks, require leak-free safe operation, known-mixture volume recovery within a predeclared tolerance (initial target ≤5% of oil volume, refined to instrument resolution), stable repeatability, and evidence that the best action actually changes across realistic conditions. Reject if passive/PID control is already near the attainable recovery/storage tradeoff or if ML only predicts oil visibility. A later confirmatory target might be ≥15% more oil before the same collection-volume limit without increased measured energy, while reporting all phase-separation failures, but that is a design goal, not a predicted result or universal statistical threshold.

**Geography/impact:** Relevant to sheltered marine/estuarine spill response and also inland water. Saltwater transfer needs separate contained validation. The small apparatus cannot demonstrate open-ocean capability, ecosystem recovery or reduced toxicity. **Verdict:** Feasible apparatus within budget, but only a conditional research choice; novelty risk is higher than construction risk.


**Energy and action-data checks:** the budget must include an inline DC current/voltage measurement module with a calibration check against a known load; allocate it from the controller/electronics line before purchase. Record all powered motors/paddle loads consistently, distinguishing common test-wave energy from intervention energy. Do not equate commanded speed with measured energy. Original development runs must vary actions under comparable disturbance conditions, so the model learns action consequences rather than merely identifying a wave-sequence label. Compare methods at a predeclared collection-volume/time/energy envelope and retain early failures. The outcome is delivered test oil in the collection container, not a visual estimate that oil vanished from the water.

## Schedule and rules


Finish student-written SRC materials before the November 13 final application deadline; submission is not approval. Restrict any preapproval work to permitted literature/design planning. After approval, allocate two weeks for apparatus/measurement feasibility, four weeks for development and design/model selection, three weeks for frozen comparisons, and one week for repeat failures/analysis. Aim to finish core data by late January and leave February for student-authored presentation. These notes do not substitute for SRC guidance, and the timeline is contingent on actual approval and reliable pilots.

Both projects involve powered hardware, water and fabrication; the oil project additionally involves chemicals and contained waste. Disclose equipment, materials, fabrication/laser use and mentor roles and complete the forms the SRC requires. No ocean deployment or living coral/vertebrate experiment is assumed. Fair display should use a dry device and recorded tests. These are AI-assisted family research notes; the student must independently read sources, develop the plan and author submitted materials. [Official dates](https://science-fair.org/students-parents/important-dates/), [SRC](https://science-fair.org/rules-and-registration/src/), [2027 AI/rule changes](https://science-fair.org/2027-changes-from-previous-rules-procedures/).


[All project ideas](../../README.md) · [Rules and timeline](../../research/rules-and-timeline.md) · [Validation and selection](../../research/validation-and-selection.md)
