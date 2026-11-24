# Executive summary

**Public edition v1.1 · 24 November 2026**

This is a proprietary project for interactive worlds that people can create, inhabit, evolve, and observe. Its product vision connects a world editor, inhabitable spaces, situated residents, and observation tools in a simple loop: **create → inhabit → evolve → observe → modify**.

The underlying engine and implementation recipes remain private. This public dossier describes the architecture and product direction at a high level. It does not include source code, exact seeds, configurations, internal commands, raw traces, execution saves, personal data, or internal paths. It is informational project documentation, not a software release.

The system brings together distinct areas such as materials and motion, environment, chemistry, body needs, perception, memory, locomotion, and group organization. Each keeps its own rules and measures. A connection shown in a diagram is not by itself evidence that an effect is active; demonstrations describe what was observed in specific internal test scenarios.

The project’s technical contribution is the coupling of specialized mechanisms in a shared causal world with an experimental loop: recorded causes can be followed across domains, a scenario can be resumed, and branches can be compared to examine whether removing a mechanism changes later outcomes. Current demonstrations cover selected connected modules and scenarios; automatic integration of arbitrary external models remains to be established. Detailed contracts and implementation recipes remain private.

The runtime now uses declared access and timing boundaries for its inventoried components. Of 71 components across 44 phases, 49 are classified as reference-step updates, 17 as elapsed-time updates, and 5 as mixed. Thirty-two do not receive `dt` directly; two remain without direct `dt`: a lagged anatomy projection and a discrete fabrication stage, neither of which is a direct rate. Three mechanisms now scale with elapsed time under rate assumptions that have not been calibrated; one retains a discrete threshold division. The static inventory checks declared contracts, not dynamic correctness or universal physical synchronization.

The targeted suite for subdivision, thresholds, and checkpoint-resume passes **14/14 tests**. Its scope is specific: protocell uptake without division, cohesion under a constant target, organizational maintenance and recovery, and checkpoint replay. Protocell division trajectories have not been compared across all partitions; rates remain uncalibrated, and general trajectory equivalence is not claimed.

The project has targeted internal test campaigns across several areas. A general inventory listed 1,635 cases, but that run did not produce a complete report. Completed targeted batches include 122/122 numerical physics checks, 80/80 checks across several domestic, causal, and chemical areas, 192/192 checks in a body, perception, memory, and simulated-resident batch, 40/40 workspace checks, 31/31 domestic hydrology checks, and 11/11 engine coordination checks. These batches may overlap and must not be added into one total. They describe internal results under defined conditions, not an independent assessment of the entire system.

Several creation, observation, habitat, and embodiment functions are under development or checked in targeted flows. The full product loop is not yet available as one continuous, durable application. Known work includes persistence, navigation, access to resources, long-session usability, and consistent timing across domains. Ideas such as causal variation, selective forgetting, and memory reconstruction remain design directions until they measurably affect later decisions.
