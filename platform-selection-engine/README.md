# The Platform Selection Engine

![Type](https://img.shields.io/badge/Type-Decision%20Framework-blue)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

**Key takeaway:** An original, weighted, dollar-based decision framework for high-stakes platform and vendor selection. It resolves every capability and every external cost into a bounded dollar figure, separates the sticker-price question from the true total-cost-of-ownership question, and carries the decision all the way through to an executive readout. The method is domain-agnostic; a data-warehouse / ML-platform selection and a CRM selection are used as worked examples.

**Role:** Author, Framework Designer
**Methods:** Weighted multi-criteria decision analysis, TCO modeling, PERT three-point estimation, AHP criteria weighting, Monte Carlo simulation, sensitivity analysis

---

## Deliverable

**Full Framework:** [the-platform-selection-engine.pdf](./the-platform-selection-engine.pdf)
*(Large file, click the link above, and if it does not display immediately, use the Download button left of the pencil icon on the right-hand side of the screen to view.)*

---

## Overview

Most platform decisions are made on sticker price and a feature checklist. This framework argues that both are misleading: bundled pricing hides the true cost, and a capability that technically exists but needs a three-week build is not the same as one that works on day one. The engine is a repeatable method for turning a messy, high-stakes selection into a defensible, dollar-based recommendation a leadership committee can act on.

It is built to be domain-agnostic. The same machinery that compares data-warehouse and ML platforms (for example Snowflake, SageMaker, and Databricks) applies to CRM vendor selection or any other enterprise-platform decision.

## Core Philosophy

Five rules govern the whole engine:

- **One shared baseline.** Every vendor is priced off the same organization numbers and the same basket of capabilities, so the comparison is valid even if a volume estimate is imperfect.
- **Everything resolves to a dollar figure.** Each feature and each external force becomes a number or a bounded range. No "it depends" survives.
- **Three separate verdicts, in sequence:** a features-only winner, an external-cost winner, and a combined-cost winner. The insight usually lives in where they disagree.
- **Verified vs. estimated, always labeled.** [SOURCED] for confirmed figures, [EST] for modeled ones, with bounds on anything uncertain.
- **Bounds discipline.** Uncertain figures use optimistic / most-likely / pessimistic estimates and a PERT expected value, rather than false precision.

## How It Works

The framework runs in phases:

- **Frame the decision** (trigger, success criteria, horizon, hard constraints and knockout criteria)
- **Build the shared baseline** (a scale vector and a usage-frequency vector that drive every cost formula)
- **Enumerate requirements** to the individual feature, tagged must-have vs. nice-to-have and weighted by category
- **Price every feature per vendor** using an atomic cost formula that accounts for tier upgrades, add-ons, consumption metering, and hidden fees, then roll up likely-use, future-looking, and full-ceiling totals
- **Quantify external costs** (implementation, data migration, integration, skills and hiring, ramp time, adoption risk, security, lock-in, downtime, support, opportunity cost)
- **Combine, score, and validate** with a weighted scoring matrix, a sensitivity/bounds test, and a pilot before committing
- **Recommend answer-first** and communicate the decision at the right depth for each audience

## Quantitative Methods

The framework formalizes each step where possible:

- **TCO and net-value equations** across features, external costs, and benefits over a fixed horizon
- **PERT three-point estimation** (E = (O + 4M + P) / 6) for every uncertain input
- **AHP (Analytic Hierarchy Process)** to derive criteria weights from pairwise comparisons, with a consistency-ratio check
- **Weighted Sum Model** scoring with normalized criteria
- **Monte Carlo simulation** to convert bounded estimates into a probability that each vendor is the best choice
- **Sensitivity analysis:** tornado / one-way sensitivity, break-even thresholds, weight-swing tests, and scenario analysis
- **Optional advanced methods:** Expected Value of Perfect Information, NPV/IRR, TOPSIS as a scoring cross-check

## Communication Layer

The framework treats the executive readout as load-bearing as the math: audience laddering (board vs. steering committee vs. working team), an answer-first deck architecture where every slide title states the takeaway, slide-time discipline, and honesty markers (labeled sources, shown bounds, stated counter-cases) that build trust with a decision-making committee.

## How to Navigate

- Read the **full framework PDF** for the complete methodology, phase by phase, plus the quantitative layers and the evidence base behind each principle.
- The framework is written to be run: each phase includes what to produce and where to find the real numbers.
