# DeepML Specialized Topic Atlas

The atlas turns all 42 corpus topics into navigable language-reference cards.

## Adapter

Defines an explicit, versioned conversion from one domain representation to another without erasing units or provenance.

- **Corpus records:** 143
- **Publication roles:** 135 positive; 8 diagnostic; 0 certification
- **Tiers:** 1
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** declare_adapter

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Calibration

Associates observations and models through a versioned calibration state, objective, tolerance, uncertainty, and evidence record.

- **Corpus records:** 188
- **Publication roles:** 164 positive; 24 diagnostic; 0 certification
- **Tiers:** 2
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_calibration

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Calibration Folding

Folds fixed calibration constants into a graph only when validity range, version, and equivalence remain provable.

- **Corpus records:** 187
- **Publication roles:** 148 positive; 39 diagnostic; 0 certification
- **Tiers:** 5
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** optimize_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Constraint

Declares a typed invariant or admissibility condition and identifies the stage responsible for enforcement.

- **Corpus records:** 188
- **Publication roles:** 174 positive; 14 diagnostic; 0 certification
- **Tiers:** 2
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_constraint

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Custom Op Hash Mismatch

Certification case requiring an implementation or artifact hash mismatch to invalidate the operator.

- **Corpus records:** 143
- **Publication roles:** 0 positive; 0 diagnostic; 143 certification
- **Tiers:** 6
- **Expected stages:** runtime_validation
- **Semantic operators:** certify_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Custom Operator

Introduces a governed domain operator with a stable signature, effect set, hash, implementation boundary, and replay contract.

- **Corpus records:** 143
- **Publication roles:** 136 positive; 7 diagnostic; 0 certification
- **Tiers:** 1
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** declare_custom_operator

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Differentiable Simulation

Exposes simulation dynamics to gradient-based reasoning while retaining integrator, stability, causality, and replay evidence.

- **Corpus records:** 417
- **Publication roles:** 357 positive; 60 diagnostic; 0 certification
- **Tiers:** 3
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_differentiable_simulation

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Dimensional Simplification

Reduces compound units only when the transformation is exact, traceable, and semantically safe.

- **Corpus records:** 188
- **Publication roles:** 152 positive; 36 diagnostic; 0 certification
- **Tiers:** 5
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** optimize_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Domain Inference

Infers a domain interpretation from declared evidence rather than from naming or output appearance alone.

- **Corpus records:** 417
- **Publication roles:** 349 positive; 68 diagnostic; 0 certification
- **Tiers:** 3
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_domain_inference

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Domain Metadata

Carries domain identity, policy, provenance, confidence, and compatibility information through compilation and runtime.

- **Corpus records:** 143
- **Publication roles:** 136 positive; 7 diagnostic; 0 certification
- **Tiers:** 1
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** declare_domain_metadata

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Domain Pack

Bundles schemas, tensors, operators, adapters, policies, and evidence as a versioned reusable domain package.

- **Corpus records:** 143
- **Publication roles:** 136 positive; 7 diagnostic; 0 certification
- **Tiers:** 1
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** declare_domain_pack

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Domain Tensor

Declares unit-bearing multidimensional data inside a named domain and preserves shape, provenance, and domain identity.

- **Corpus records:** 143
- **Publication roles:** 136 positive; 7 diagnostic; 0 certification
- **Tiers:** 1
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** declare_domain_tensor

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Domain Validation

Checks that a domain package is internally coherent before optimization, lowering, or execution.

- **Corpus records:** 187
- **Publication roles:** 171 positive; 16 diagnostic; 0 certification
- **Tiers:** 2
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_domain_validation

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Finance Operator

Models financial transformations with currencies, horizons, assumptions, risk semantics, and no-network defaults.

- **Corpus records:** 187
- **Publication roles:** 166 positive; 21 diagnostic; 0 certification
- **Tiers:** 2
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_finance_operator

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Forbidden Market Network

Certification case requiring the no-network policy to block live market access.

- **Corpus records:** 143
- **Publication roles:** 0 positive; 0 diagnostic; 143 certification
- **Tiers:** 6
- **Expected stages:** semantic_validation
- **Semantic operators:** certify_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Graphics Operator

Encodes deterministic graphics-domain transformations with explicit inputs, outputs, units, tolerances, and effects.

- **Corpus records:** 188
- **Publication roles:** 174 positive; 14 diagnostic; 0 certification
- **Tiers:** 2
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_graphics_operator

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Graphics Pipeline

Transforms simulation or domain state into graphical evidence without confusing rendering with latent semantic truth.

- **Corpus records:** 416
- **Publication roles:** 375 positive; 41 diagnostic; 0 certification
- **Tiers:** 4
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** integrate_graphics_pipeline

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Hybrid Domain Package

Publishes a cross-domain graph and its adapters, policies, dependencies, and evidence as one bounded artifact.

- **Corpus records:** 417
- **Publication roles:** 375 positive; 42 diagnostic; 0 certification
- **Tiers:** 4
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** integrate_hybrid_domain_package

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Invalid Constraint

Certification case requiring rejection of inconsistent, unsatisfied, or ill-typed constraints.

- **Corpus records:** 143
- **Publication roles:** 0 positive; 0 diagnostic; 143 certification
- **Tiers:** 6
- **Expected stages:** semantic_validation
- **Semantic operators:** certify_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Kernel Selection

Chooses a compatible implementation using deterministic rules, capability checks, and stable identity.

- **Corpus records:** 187
- **Publication roles:** 152 positive; 35 diagnostic; 0 certification
- **Tiers:** 5
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** optimize_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Multidomain Graph

Coordinates multiple domain namespaces and adapters in one typed, policy-governed computation graph.

- **Corpus records:** 416
- **Publication roles:** 350 positive; 66 diagnostic; 0 certification
- **Tiers:** 3
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_multidomain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Noncausal Simulation

Certification case requiring noncausal dependencies or future-state leakage to be rejected.

- **Corpus records:** 142
- **Publication roles:** 0 positive; 0 diagnostic; 142 certification
- **Tiers:** 6
- **Expected stages:** semantic_validation
- **Semantic operators:** certify_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Op Specialization

Specializes a generic operator for a domain, type, shape, or target without changing its declared meaning.

- **Corpus records:** 187
- **Publication roles:** 147 positive; 40 diagnostic; 0 certification
- **Tiers:** 5
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** optimize_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Portfolio Risk

Computes bounded portfolio-risk evidence under explicit horizon, currency, scenario, and input-provenance contracts.

- **Corpus records:** 417
- **Publication roles:** 375 positive; 42 diagnostic; 0 certification
- **Tiers:** 4
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** integrate_portfolio_risk

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Provenance Kernel

Makes origin, transformation history, hashes, and evidence propagation part of the executable semantics.

- **Corpus records:** 416
- **Publication roles:** 359 positive; 57 diagnostic; 0 certification
- **Tiers:** 3
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_provenance_kernel

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## R12 Mcrt Lowering

Emits stable relations, operators, confidence, status, provenance, and replay identities for downstream JA21 layers.

- **Corpus records:** 188
- **Publication roles:** 148 positive; 40 diagnostic; 0 certification
- **Tiers:** 5
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** optimize_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Risk Physics Coupling

Connects physical state and risk state without silently conflating units, causality, uncertainty, or judgement.

- **Corpus records:** 417
- **Publication roles:** 351 positive; 66 diagnostic; 0 certification
- **Tiers:** 3
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_risk_physics_coupling

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Robotics Operator

Represents sensing, estimation, planning, or control while keeping physical authority and safety boundaries explicit.

- **Corpus records:** 188
- **Publication roles:** 167 positive; 21 diagnostic; 0 certification
- **Tiers:** 2
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_robotics_operator

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Robotics Stack

Connects sensing, fusion, planning, and declaration-only control under explicit safety and actuation gates.

- **Corpus records:** 417
- **Publication roles:** 375 positive; 42 diagnostic; 0 certification
- **Tiers:** 4
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** integrate_robotics_stack

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Schema

Defines structured domain data with named fields, types, units, timestamps, provenance, and validation obligations.

- **Corpus records:** 142
- **Publication roles:** 135 positive; 7 diagnostic; 0 certification
- **Tiers:** 1
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** declare_schema

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Scientific Operator

Captures scientific transformations with units, uncertainty, calibration, provenance, and reproducibility requirements.

- **Corpus records:** 187
- **Publication roles:** 163 positive; 24 diagnostic; 0 certification
- **Tiers:** 2
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_scientific_operator

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Scientific Workflow

Composes local datasets, calibrated operators, uncertainty, and reproducibility evidence into a scientific pipeline.

- **Corpus records:** 417
- **Publication roles:** 375 positive; 42 diagnostic; 0 certification
- **Tiers:** 4
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** integrate_scientific_workflow

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Sensor Fusion

Combines heterogeneous observations under explicit frames, units, timestamps, confidence, and provenance.

- **Corpus records:** 417
- **Publication roles:** 359 positive; 58 diagnostic; 0 certification
- **Tiers:** 3
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_sensor_fusion

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Simulation Environment

Defines initial state, step policy, causal schedule, boundary conditions, and deterministic replay for simulation.

- **Corpus records:** 416
- **Publication roles:** 375 positive; 41 diagnostic; 0 certification
- **Tiers:** 4
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** integrate_simulation_environment

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Simulation Operator

Advances a declared simulation state under an explicit time model, causal order, integrator, and validation profile.

- **Corpus records:** 187
- **Publication roles:** 171 positive; 16 diagnostic; 0 certification
- **Tiers:** 2
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** compose_simulation_operator

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Sparse Planning

Builds an efficient execution plan for sparse graphs while preserving dependencies, determinism, and evidence.

- **Corpus records:** 187
- **Publication roles:** 148 positive; 39 diagnostic; 0 certification
- **Tiers:** 5
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** optimize_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Target Lowering

Maps specialized semantics into a declared backend representation while preserving units, policies, hashes, and provenance.

- **Corpus records:** 188
- **Publication roles:** 153 positive; 35 diagnostic; 0 certification
- **Tiers:** 5
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** optimize_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Unit Mismatch

Certification case requiring dimensional inconsistency to fail at the earliest responsible stage.

- **Corpus records:** 143
- **Publication roles:** 0 positive; 0 diagnostic; 143 certification
- **Tiers:** 6
- **Expected stages:** type_check
- **Semantic operators:** certify_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Unit Propagation

Carries dimensional information through graphs and rejects operations that cannot preserve or intentionally convert it.

- **Corpus records:** 188
- **Publication roles:** 152 positive; 36 diagnostic; 0 certification
- **Tiers:** 5
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** optimize_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Unit Type

Treats physical, financial, robotic, graphical, biological, and other domain units as semantic types rather than comments.

- **Corpus records:** 143
- **Publication roles:** 136 positive; 7 diagnostic; 0 certification
- **Tiers:** 1
- **Expected stages:** runtime, semantic_validation
- **Semantic operators:** declare_unit_type

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Unsafe Actuation

Certification case requiring rejection of undeclared or unauthorized physical actuation.

- **Corpus records:** 143
- **Publication roles:** 0 positive; 0 diagnostic; 143 certification
- **Tiers:** 6
- **Expected stages:** safety_gate
- **Semantic operators:** certify_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.

## Unstable Calibration

Certification case requiring calibration instability or out-of-range use to be rejected or quarantined.

- **Corpus records:** 143
- **Publication roles:** 0 positive; 0 diagnostic; 143 certification
- **Tiers:** 6
- **Expected stages:** runtime_validation
- **Semantic operators:** certify_domain_graph

**Engineering lens:** preserve domain identity, units, schemas, provenance, deterministic evaluation, no-network policy, explicit authority, calibrated tolerances, and R12/MCRT evidence.
