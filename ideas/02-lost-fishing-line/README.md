# Remove lost fishing line without pulling it tighter

Research reviewed October 22–23, 2026. AI-assisted family background research; no prototype or cleanup result has been validated.

**Scope:** a contained sequential disentanglement component, not a complete underwater robot. All budget items are purchasing allowances. Existing printer, laser cutter and computer are excluded. The $855 base allowance assumes access to a phone camera; add a $40 USB-camera allowance if needed, for $895 total.


### The problem and current removal practice

Lost fishing gear can keep entangling organisms and abrading, breaking or shading reef habitat. [NOAA's account of its original reef survey](https://www.fisheries.noaa.gov/index.php/feature-story/impacts-ghost-nets-coral-reefs) describes lower live-coral cover at net-affected sites. Removing a net does not immediately restore that cover: [a subsequent NOAA-hosted 2023 study](https://repository.library.noaa.gov/view/noaa/49278) reports suppression persisting three years after removal. The relevant direct endpoint is removing the gear, not claiming rapid coral recovery.

The problem is current and locally understandable: [Ghost Diving USA's 2026 Southern California project](https://www.ghostdivingusa.org/the-midnight-hour) cuts and lifts netting from the Midnight Hour wreck. Its technical divers remove sections by hand, rather than dragging them free. A [DTU field-removal report](https://www.aqua.dtu.dk/-/media/institutter/aqua/publikationer/rapporter-352-400/appendices_ghost-nets-in-danish-waters.pdf) likewise describes planning cuts, freeing the material and attaching lift bags. These are professional operations, not proposed student field activities.

### A genuinely different student-scale engineering question

**Can a small retrieval head learn which short pull–slacken–redirect sequence frees entangled line under a fixed tension/time limit, more reliably than a tuned multidirectional search?** The target is already-lost material being removed. This is not low-shedding operation of a fishing hauler and not a single classify-and-pick action.

Build a fixed benchtop wet-test head with two small motion axes or a comparably simple cable-driven mechanism. A soft clamp holds one known line/net edge. The head can make a few bounded moves, release tension and change direction. The test fixture has interchangeable branching obstacles, and all material remains in a catch tray. A complete ROV, autonomous navigation, underwater motor sealing and automated cutting are deliberately outside the prototype. Initially restrict the task to entanglements that can physically be removed without cutting; include impossible/unrecoverable layouts in the test denominator as failures rather than silently excluding them after testing.

This restricted task has an important practical limitation: much real ghost gear must be cut, is biofouled or is attached to organisms. A successful prototype would be a retrieval-component experiment, not a substitute for trained divers or demonstrated field cleanup. Whether this restricted subtask is useful enough for field operators remains unverified; do not claim otherwise.

### Prior research/commercial comparison and the possible gap

- [NETTAG+ IRIS](https://www.nettagplus.eu/resources/) already localizes gear and mechanically secures it or attaches a recovery line. The [EU's current project account](https://cinea.ec.europa.eu/featured-projects/nettag-turning-lost-fishing-gear-action-healthier-european-seas_en?prefLang=sl) describes the programme's deployed technology. Robotic gear recovery itself is established.
- [Ghost Gear Disappear's commercial retrieval service](https://www.ghostgeardisappear.com/pages/services/ghost-gear-retrieval) already uses sonar/video-guided ROV attachment, explicitly distinguishing it from indiscriminate bottom dragging. Its shop offers grippers; manufacturer/service descriptions are evidence of existing capability, not independent performance validation.
- Learned cable disentanglement is also established: [Viswanath et al., 2022](https://arxiv.org/abs/2207.07813) and [Sundaresan et al., 2021](https://arxiv.org/abs/2107.08942) use perception/manipulation primitives and recovery policies. Do not claim the first ML untangling system.

**Possible narrow contribution:** physical validation of a low-cost, force-constrained recovery policy on previously unseen line–branch arrangements, including failed attempts and material still attached. This search did not verify a near-identical low-cost experiment, but absence from a search does not establish global novelty. The field-transfer gap remains substantial.

### Where ML might earn its place

Use a small regularized tree/GP outcome model, not end-to-end robot learning. It estimates the chance of progress and tension increase for each permitted move from a short trial pull, force–displacement response, visible line direction/crossings and obstacle descriptors. It then physically executes a move, reassesses and continues. Original randomized action trials supply the labels; photographs alone do not supply action consequences.

The hard baselines are the **same hardware** using: (1) an optimized fixed pull direction; (2) a force-limited rule that slackens and tries directions in a tuned order; and (3) a simple geometric/linear action model. Give all methods the same sensing, tuning opportunities, action count, tension cap and total time. If ordinary slacken-and-search matches recovery, stop the ML claim. A model trained to recognize the deliberately assigned tangle ID would be a shortcut, not useful learning.

### Ground truth, independent tests and claim limits

Use documented commercial fishing-line/net materials, not unknown retrieved gear or live habitat. Measure known starting dry polymer mass/line length, complete gear recovery to a separate container, remaining attached material, broken detached pieces and every unsuccessful episode. A partially loosened net still attached to the fixture is not removed pollution. Primary outcomes: fully recovered mass or successful complete recovery, time, attempts and peak measured pull tension. Retained fraction and broken pieces must be reported, not hidden in a success rate.

Calibrate tension using known loads and check force–displacement timing. A sensor at the gripper measures gripper-line tension; it does not measure every local contact force. Fixture reaction measurements and sacrificial-obstacle breakage may characterize the apparatus, but **printed/plaster branches do not validate coral injury reduction**. A selected tension cap is a mechanical test constraint, not a biologically safe limit. Do not make a microplastic-emissions claim: basic mass/count methods will not resolve all small abrasion products.

After a small pilot, develop on roughly 40–60 separately prepared entanglement episodes, with repeated moves nested inside episodes. Freeze models and rules before approximately 36–48 confirmation episodes distributed across all four policies and new fixture geometries, line/net batches and entanglement families. One starting allocation is four policies × three held-out entanglement families × three freshly prepared episodes = 36; increase repeats according to pilot variability rather than treating three as a power calculation. Randomize by session; hold whole episodes/families out, never adjacent video frames. Counts are a planning scale, not a power calculation. A small number of independently varied tangle families limits generalization even if thousands of force samples are logged.

### Full planning budget and schedule

| Item | USD allowance |
|---|---:|
| Fixed two-axis mechanism/frame | 160 |
| Soft clamp and replaceable contact surfaces | 60 |
| Motors/drivers/power | 100 |
| Load cells, controller, position sensing and calibration loads | 110 |
| Catch trays, interchangeable printed fixtures, replacement parts | 75 |
| Documented line/net materials | 45 |
| Basic balance and mass/length checks | 50 |
| Camera mounting, lighting, collection bags/screens | 25 |
| Guards/PPE | 25 |
| Fair entry | 40 |
| Tax/shipping | 65 |
| Contingency/display printing | 100 |
| **Total** | **855** |

This budget supports gram-scale gear recovery and mechanical force measurements; it does not buy coral testing, an ROV or validated microplastic analysis. Begin physical pilots only after any required SRC approval. Spend the first 7–10 approved testing days on a crude mechanism and recovery cases, then 3–4 weeks on the finite action/data set and 3–4 on frozen comparisons. Reserve January for held-out trials and repairs; no field access is assumed.

**Pros:** existing harmful material is physically removed; no ongoing harmful industry needs to become more productive; no chemical assay or animal work; fixtures and documented line can be tested indoors in winter.

**Cons/mitigation:** robot untangling and ROV recovery are mature—make the benchmark unusually transparent and modest, not a first-invention claim. Restrict mechanism complexity to the two-axis head and finite moves. Real nets are more complex than the test—state that limit, and do not call a new-net fixture a reef restoration experiment. Wet friction/occlusion may defeat perception—include them as test conditions rather than hiding them with an easy colour label.

**Kill within the pilot** if removing representative uncutted layouts requires more axes/regrasping than the budgeted mechanism, if a single force threshold plus direction search solves the cases, if only hand-selected easy tangles can be released, or if outcomes are dominated by the manufactured fixture rather than line configuration. Before calling it a strong environmental-engineering contender, demonstrate a held-out recovery improvement exceeding between-episode variation at the same time/force limits. No numerical improvement is promised.

**Decision:** conditional, moderate mechanical risk and high novelty/application risk. It is a different *sequential disentanglement* question from archived 24/25, but a plain gripper pulling visible litter would be a rebrand and is rejected.

## Schedule and rules

Allow roughly two approved pilot weeks, three to four development weeks and three to four frozen-comparison weeks, with time for repairs and analysis. No field gear retrieval, live habitat work or protected-site access is part of the core. Disclose the moving mechanisms, force limits, water/electricity, fabrication and disposal in the actual SRC protocol. Experimental work requiring prior authorization begins only after approval. A dry mechanism, recordings and data can be used at the fair; water and live habitat cannot.

[Comparison and selection](../../README.md) · [Shared rules](../../research/rules-and-timeline.md) · [Validation requirements](../../research/validation-and-selection.md)
