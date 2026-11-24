# Interactive Worlds — short edition

**Public edition v1.1 · 24 November 2026**

**Language:** English · [Lire en français](../Presentation_mondes_interactifs_lite_v1.1.md) · [Home](../index_en.html)

> **In 30 seconds** — A proprietary project for interactive worlds that people can create, inhabit, and observe. The engine and implementation recipes remain private. This repository contains public documentation, presentation diagrams, and high-level results only. It includes no source code, configuration, or raw data.

## The idea

An interactive world is more than a scene on a screen. It contains places, objects, resources, inhabitants, and relationships that can change over time. The project aims to bring these elements into one environment: someone shapes a place, gives its inhabitants a situation to explore, starts the world, and then observes what has changed.

The product vision follows a simple loop: **create → inhabit → evolve → observe → modify**. A world editor is intended to compose spaces and objects. Habitats give places rooms, passages, and access constraints. Inhabitants can perceive, move, retain traces of experience, and act within their surroundings. Observation tools help people follow changes and recorded interactions.

These elements are at different stages. Several functions and user flows have been built and checked separately; they are not yet all joined into one continuous, durable experience.


## How the system connects mechanisms

### What the project contributes

The project makes composition a testable experiment loop: selected specialized mechanisms share one world, their recorded consequences can be followed across domains, and resumed or compared branches help examine whether a mechanism changes a later action. This continuity between composition, causal provenance, and intervention is the project’s technical proposition.

Reported results cover the modules and scenarios actually connected. The project does not claim automatic integration of any third-party model or universal validity of its grammar. Detailed contracts, parameters, and implementation recipes remain private.

The runtime uses access and timing contracts for its inventoried components. The static inventory covers 44 phases and 71 components: 49 are classified as reference-step updates, 17 as elapsed-time updates, and 5 as mixed. Of the 32 that do not receive `dt` directly, 2 remain without direct dt: one lagged anatomy projection and one discrete fabrication stage, neither a direct rate. Three mechanisms now scale with elapsed time under rate assumptions that have not been calibrated; one retains a discrete threshold division. A common world order connects mechanisms without forcing them onto one identical cadence. This check covers declared boundaries, not physical synchronization or the complete behavior of every chain.

The targeted suite for subdivision, thresholds, and checkpoint-resume passes **14/14 tests**. Its scope is specific: uptake without division, cohesion under a constant target, organizational maintenance and recovery, and checkpoint replay. Protocell division trajectories have not been compared across all partitions; rates remain uncalibrated and general trajectory equivalence is not claimed.

The system brings together areas with their own rules: materials and movement, water and environment, chemistry, bodily needs, perception, memory, locomotion, and group organization. They can share a world without sharing the same units or update pace.

To examine an interaction, a test follows an initial state, the relationships that let mechanisms act, the changes they produce, and the observations available afterward. A remembered trace, for example, affects behavior only when a mechanism reads it and a later decision or action changes as a result. Showing a connection between two areas does not by itself show that an effect is transmitted.

This way of describing the system helps ask practical questions: which element holds the state? Which mechanism changes it? What interaction links two parts? What change can be observed afterward? Each area keeps its own measures and rules.

## Create and explore a world

The intended product experience starts with an editor for composing a place, its objects, and its initial conditions. Habitable spaces add rooms, access routes, and household functions. Inhabitants and embodied doubles provide a situated point of view: they can appear in a place, receive signals, move, and take part in some interactions.

Observation tools make trajectories easier to explore through scenes, maps, views, and recorded events. They help answer practical questions: what changed? Which inhabitant or resource is involved? What other trajectory can be compared? An image can make a world easier to read, but the underlying states and events remain the source of what it shows.

Over time, the goal is to create a world, save it, resume it, follow its history, and modify it while preserving useful continuity. Persistence, navigation, access to resources, and long-session usability remain work in progress.

## What the system has already run

The system is not a single module judged by one global score. It combines a states–relationships–dynamics framework, a causal experimental engine, specialized domains, and tools for creating and observing scenarios. The full dossier maps 11 theoretical formulations with different statuses, five cascade questions, a 23-scale research map, synthetic hysteresis measurements, event identifiers, checkpoints and replay, then domain families, their connections, and their campaigns. The 23 scales are not all simulated, and the 11 formulations are not all validated. The short results below illustrate several kinds of capability; they do not summarize the full corpus.

**Mechanisms co-act in a shared world.** In a garden campaign, a retained experience contributes to a route and a later irrigation action. Matched branches where that memory contribution is removed do not produce the same action; the contrast was reproduced across multiple initializations. Other scenarios bring memory, bodily state, and group organization together. A group scenario follows how feedback changes resource allocation and an individual member's decision.

**Long campaigns expose failures as well as behavior.** In an instrumented subsistence scenario running for about two hours, trajectories diverged and the group dissolved in one branch at step 1,855 of a 2,160-step horizon. The post-mortem links part of this outcome to movement blockages and effective access to resources. That run reached nearly **3.8 GiB of RAM** and generated more than one million events in its most heavily instrumented branch: this measures the cost of that scenario and its logging, not the engine's maximum capacity.

**Targeted batches cover several domains.** Completed documented batches include **122/122** numerical physics checks; **80/80** checks across domestic, causal, and chemical areas; **192/192** checks in a body, perception, memory, and resident batch; **40/40** workspace checks; **31/31** domestic hydrology checks; and **11/11** engine coordination checks. Locomotion, optics, ecology, hearing, and vision campaigns add comparisons with domain-specific criteria. For example, 50 of 75 scenes were retained in the visual evaluation and 2 of 5 repetitions met its full internal criterion; six evaluated joint trajectories were closer to the reference than the neutral pose.

A broad inventory listed **1,635 cases** but did not produce a complete report. The targeted batches are different, sometimes overlapping records, so they do not form one additive total. They show the breadth of work and internal results under defined conditions, not uniform maturity or an independent evaluation of the whole system.

A separate execution record publishes filtered time series: **47.99 hours**, **2,873 samples**, **416 net ticks** during monitoring (from **809 to 1,225**), and **0.87?1.32 GiB** resident memory. Private memory reached **1.77 GiB**. The process was reported alive at each sample, but no tick advanced during the **final nine minutes** of the monitored window. A separate world trace reaches tick **1,274**, without timestamps that can be aligned to the resource monitor. The monitored window ends about **50 seconds short of 48 hours**; it approaches, but does not formally meet, that threshold. Six public snapshots cannot characterize the residents? complete trajectories. This record describes that run; it does not replace the integrated behavior campaigns or the load measurement above.

## Current state and known limits

The technical foundation and several creation, observation, habitat, and embodiment tools are in development or checked in targeted flows. Demonstrations describe what is connected in those flows; they do not mean the full product vision is already available as one integrated application.

The domains do not yet share a single timing contract. Measures from one area cannot be substituted for another’s. Some results depend on specific scenarios, and campaign duration or resident count alone cannot establish the quality of every interaction. Hardware endurance and continuity across long-running worlds remain active work.

Ideas such as causal variation, selective forgetting, and memory reconstruction are design directions. They are not presented as integrated capabilities until they measurably change later decisions.

## Ownership and scope

The project is proprietary. The engine, source code, and implementation recipes remain private. This dossier describes the product direction and high-level results without distributing the means used to build it.

This edition includes no source code, exact seeds, configurations, internal commands, raw traces, execution saves, personal data, or internal paths. It presents the product direction and current state without distributing the means used to build it.

## Editions

The diagrams are conceptual and illustrate the descriptions in this dossier. The complete technical dossier contains a more detailed account of the system’s areas, demonstrations, and known limits. Both public editions are version **1.1 — 24 November 2026**.
