# JA21 DeepML Specialized Language
## Domains, Units, Evidence, and Bounded Cross-Domain Computation

**Standalone textbook for suite version 1.0.0**

> A specialized language earns trust not by producing an impressive output, but by preserving the meaning, units, provenance, authority, causality, and evidence of every transformation that produced it.

### Editorial council

- **SOPHIA:** semantic integrity, dimensional consistency, claim boundaries, domain invariants, and evidence discipline.
- **CHARLOTTE:** corpus taxonomy, cross-domain terminology, learning architecture, indexing, and editorial coherence.
- **LANDON:** compiler/runtime contracts, deterministic replay, safety gates, diagnostics, and package engineering.
- **Professor:** technical pedagogy, laboratories, assessment, curriculum sequencing, and textbook coherence.
- **Podium:** publication quality, visual hierarchy, navigability, release presentation, and institutional finish.

## How to use this book

Read the chapters in sequence for a course, or use the topic atlas and reading paths for role-based study. Every chapter combines a corpus-derived program, conceptual explanation, engineering controls, a laboratory, evidence requirements, and review questions. Positive examples demonstrate admitted behavior. Diagnostic examples demonstrate required rejection. Certification holdouts are reserved for frozen-implementation evaluation.

## Claim and execution boundary

The textbook describes a language and evidence architecture reconstructed from the supplied corpus. It does not claim that a native compiler, simulator, financial engine, graphics renderer, robotic controller, or physical theory has been independently implemented or validated. The Smithson 8S material is presented as a proposed computational framework with explicit limitations.

---

# Chapter 1: The Specialized Language as a JA21 Suite

## Learning objectives

- Explain the role of language identity, evidence chains, and the boundary between domain code and narrative labels in the DeepML Specialized evidence chain.
- Author and inspect a bounded domain tensor program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

The Specialized Language as a JA21 Suite is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **language identity, evidence chains, and the boundary between domain code and narrative labels**. Declares unit-bearing multidimensional data inside a named domain and preserves shape, provenance, and domain identity. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_00001
policy deterministic
policy no_network
domain finance {
  unit U1 = base("finance")
  schema Sample00001 { value: f64<U1> timestamp: Time provenance: Hash }
  tensor observations: f64<U1>[2,3]
  operator normalize_finance(x: Tensor<U1>) -> Tensor<Dimensionless> pure
  adapter SampleToTensor from Sample00001 to Tensor<U1>
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Trace ten records from source through AST, semantics, validation, R12, and MCRT.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct language identity, evidence chains, and the boundary between domain code and narrative labels?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 2: Domains, Namespaces, Imports, and Packages

## Learning objectives

- Explain the role of bounded namespaces, imports, reusable packages, and dependency identity in the DeepML Specialized evidence chain.
- Author and inspect a bounded domain pack program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Domains, Namespaces, Imports, and Packages is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **bounded namespaces, imports, reusable packages, and dependency identity**. Bundles schemas, tensors, operators, adapters, policies, and evidence as a versioned reusable domain package. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_00005
policy deterministic
policy no_network
domain physics {
  unit U5 = base("physics")
  schema Sample00005 { value: f64<U5> timestamp: Time provenance: Hash }
  tensor observations: f64<U5>[6,7]
  operator normalize_physics(x: Tensor<U5>) -> Tensor<Dimensionless> pure
  adapter SampleToTensor from Sample00005 to Tensor<U5>
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Design a local package that imports two domains through explicit versioned boundaries.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct bounded namespaces, imports, reusable packages, and dependency identity?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 3: Unit Types and Dimensional Integrity

## Learning objectives

- Explain the role of base units, compound units, conversions, propagation, and mismatch rejection in the DeepML Specialized evidence chain.
- Author and inspect a bounded unit type program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Unit Types and Dimensional Integrity is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **base units, compound units, conversions, propagation, and mismatch rejection**. Treats physical, financial, robotic, graphical, biological, and other domain units as semantic types rather than comments. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_00003
policy deterministic
policy no_network
domain graphics {
  unit U3 = base("graphics")
  schema Sample00003 { value: f64<U3> timestamp: Time provenance: Hash }
  tensor observations: f64<U3>[4,5]
  operator normalize_graphics(x: Tensor<U3>) -> Tensor<Dimensionless> pure
  adapter SampleToTensor from Sample00003 to Tensor<U3>
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Create one valid unit-bearing graph and a paired mismatch diagnostic.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct base units, compound units, conversions, propagation, and mismatch rejection?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 4: Schemas, Metadata, and Provenance

## Learning objectives

- Explain the role of structured samples, timestamps, provenance hashes, metadata, confidence, and compatibility in the DeepML Specialized evidence chain.
- Author and inspect a bounded schema program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Schemas, Metadata, and Provenance is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **structured samples, timestamps, provenance hashes, metadata, confidence, and compatibility**. Defines structured domain data with named fields, types, units, timestamps, provenance, and validation obligations. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_00007
policy deterministic
policy no_network
domain robotics {
  unit U7 = base("robotics")
  schema Sample00007 { value: f64<U7> timestamp: Time provenance: Hash }
  tensor observations: f64<U7>[8,9]
  operator normalize_robotics(x: Tensor<U7>) -> Tensor<Dimensionless> pure
  adapter SampleToTensor from Sample00007 to Tensor<U7>
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Define a schema and prove that provenance survives one transformation and one adapter.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct structured samples, timestamps, provenance hashes, metadata, confidence, and compatibility?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 5: Domain Tensors and Adapters

## Learning objectives

- Explain the role of typed multidimensional observations and explicit cross-representation conversion in the DeepML Specialized evidence chain.
- Author and inspect a bounded adapter program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Domain Tensors and Adapters is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **typed multidimensional observations and explicit cross-representation conversion**. Defines an explicit, versioned conversion from one domain representation to another without erasing units or provenance. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_00002
policy deterministic
policy no_network
domain robotics {
  unit U2 = base("robotics")
  schema Sample00002 { value: f64<U2> timestamp: Time provenance: Hash }
  tensor observations: f64<U2>[3,4]
  operator normalize_robotics(x: Tensor<U2>) -> Tensor<Dimensionless> pure
  adapter SampleToTensor from Sample00002 to Tensor<U2>
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Build a tensor adapter that preserves unit, shape, timestamp, and provenance evidence.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct typed multidimensional observations and explicit cross-representation conversion?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 6: Custom Operators and Kernel Identity

## Learning objectives

- Explain the role of operator signatures, purity, effects, implementation hashes, capabilities, and deterministic selection in the DeepML Specialized evidence chain.
- Author and inspect a bounded custom operator program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Custom Operators and Kernel Identity is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **operator signatures, purity, effects, implementation hashes, capabilities, and deterministic selection**. Introduces a governed domain operator with a stable signature, effect set, hash, implementation boundary, and replay contract. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_00006
policy deterministic
policy no_network
domain finance {
  unit U6 = base("finance")
  schema Sample00006 { value: f64<U6> timestamp: Time provenance: Hash }
  tensor observations: f64<U6>[7,8]
  operator normalize_finance(x: Tensor<U6>) -> Tensor<Dimensionless> pure
  adapter SampleToTensor from Sample00006 to Tensor<U6>
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Author a custom operator profile and a hash-mismatch certification test.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct operator signatures, purity, effects, implementation hashes, capabilities, and deterministic selection?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 7: Financial Domains and Portfolio Risk

## Learning objectives

- Explain the role of currencies, horizons, scenarios, assumptions, local datasets, and risk evidence in the DeepML Specialized evidence chain.
- Author and inspect a bounded portfolio risk program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Financial Domains and Portfolio Risk is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **currencies, horizons, scenarios, assumptions, local datasets, and risk evidence**. Computes bounded portfolio-risk evidence under explicit horizon, currency, scenario, and input-provenance contracts. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_05001
policy deterministic
policy no_network
domain workflow_3 {
  graph DomainGraph05001 {
    science = scientific_pipeline(dataset="local:05001")
    portfolio = portfolio_risk(science, currency=USD)
    simulation = simulation_environment(portfolio, steps=601)
    graphics = graphics_pipeline(simulation)
    robot = robotics_control(graphics, actuation=declaration_only)
  }
  package hybrid DomainGraph05001 as "hybrid_05001.msslb"
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Construct a no-network portfolio-risk graph with explicit currency and horizon.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct currencies, horizons, scenarios, assumptions, local datasets, and risk evidence?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 8: Scientific Operators and Reproducible Workflows

## Learning objectives

- Explain the role of calibrated data, uncertainty, local datasets, reproducibility, and scientific claims in the DeepML Specialized evidence chain.
- Author and inspect a bounded scientific workflow program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Scientific Operators and Reproducible Workflows is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **calibrated data, uncertainty, local datasets, reproducibility, and scientific claims**. Composes local datasets, calibrated operators, uncertainty, and reproducibility evidence into a scientific pipeline. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_05002
policy deterministic
policy no_network
domain workflow_4 {
  graph DomainGraph05002 {
    science = scientific_pipeline(dataset="local:05002")
    portfolio = portfolio_risk(science, currency=USD)
    simulation = simulation_environment(portfolio, steps=602)
    graphics = graphics_pipeline(simulation)
    robot = robotics_control(graphics, actuation=declaration_only)
  }
  package hybrid DomainGraph05002 as "hybrid_05002.msslb"
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Build a local scientific workflow and publish its calibration and uncertainty ledger.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct calibrated data, uncertainty, local datasets, reproducibility, and scientific claims?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 9: Graphics Domains and Evidence-Preserving Pipelines

## Learning objectives

- Explain the role of graphics operators, render-facing transformations, coordinate meaning, and the difference between image and truth in the DeepML Specialized evidence chain.
- Author and inspect a bounded graphics pipeline program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Graphics Domains and Evidence-Preserving Pipelines is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **graphics operators, render-facing transformations, coordinate meaning, and the difference between image and truth**. Transforms simulation or domain state into graphical evidence without confusing rendering with latent semantic truth. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_05005
policy deterministic
policy no_network
domain workflow_0 {
  graph DomainGraph05005 {
    science = scientific_pipeline(dataset="local:05005")
    portfolio = portfolio_risk(science, currency=USD)
    simulation = simulation_environment(portfolio, steps=605)
    graphics = graphics_pipeline(simulation)
    robot = robotics_control(graphics, actuation=declaration_only)
  }
  package hybrid DomainGraph05005 as "hybrid_05005.msslb"
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Create a graphics pipeline that retains latent state and provenance beside rendered output.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct graphics operators, render-facing transformations, coordinate meaning, and the difference between image and truth?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 10: Robotics Domains, Sensor Fusion, and Authority

## Learning objectives

- Explain the role of frames, timestamps, confidence, fusion, planning, declaration-only control, and actuation gates in the DeepML Specialized evidence chain.
- Author and inspect a bounded sensor fusion program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Robotics Domains, Sensor Fusion, and Authority is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **frames, timestamps, confidence, fusion, planning, declaration-only control, and actuation gates**. Combines heterogeneous observations under explicit frames, units, timestamps, confidence, and provenance. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_02508
policy deterministic
policy no_network
domain hybrid_6 {
  import physics as P
  import finance as F
  import robotics as R
  graph DomainGraph02508 {
    state = P.differentiable_simulation(sensor_stream(provenance=sha256("2508")))
    risk = F.risk_model(state, horizon=19d)
    control = R.sensor_fusion(state, risk)
    output = domain_infer(control)
  }
  custom kernel HybridKernel hash sha256("kernel:02508") deterministic
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Fuse two sensors and prove that the result cannot trigger undeclared actuation.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct frames, timestamps, confidence, fusion, planning, declaration-only control, and actuation gates?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 11: Simulation Operators and Causal Environments

## Learning objectives

- Explain the role of state, steps, integrators, boundaries, causal schedules, replay, and noncausal rejection in the DeepML Specialized evidence chain.
- Author and inspect a bounded simulation environment program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Simulation Operators and Causal Environments is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **state, steps, integrators, boundaries, causal schedules, replay, and noncausal rejection**. Defines initial state, step policy, causal schedule, boundary conditions, and deterministic replay for simulation. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_05006
policy deterministic
policy no_network
domain workflow_1 {
  graph DomainGraph05006 {
    science = scientific_pipeline(dataset="local:05006")
    portfolio = portfolio_risk(science, currency=USD)
    simulation = simulation_environment(portfolio, steps=606)
    graphics = graphics_pipeline(simulation)
    robot = robotics_control(graphics, actuation=declaration_only)
  }
  package hybrid DomainGraph05006 as "hybrid_05006.msslb"
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Define a deterministic local simulation and a future-state leakage test.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct state, steps, integrators, boundaries, causal schedules, replay, and noncausal rejection?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 12: Domain Inference and Multidomain Graphs

## Learning objectives

- Explain the role of evidence-based inference, graph boundaries, adapters, uncertainty, and conflict handling in the DeepML Specialized evidence chain.
- Author and inspect a bounded domain inference program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Domain Inference and Multidomain Graphs is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **evidence-based inference, graph boundaries, adapters, uncertainty, and conflict handling**. Infers a domain interpretation from declared evidence rather than from naming or output appearance alone. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_02501
policy deterministic
policy no_network
domain hybrid_8 {
  import physics as P
  import finance as F
  import robotics as R
  graph DomainGraph02501 {
    state = P.differentiable_simulation(sensor_stream(provenance=sha256("2501")))
    risk = F.risk_model(state, horizon=12d)
    control = R.sensor_fusion(state, risk)
    output = domain_infer(control)
  }
  custom kernel HybridKernel hash sha256("kernel:02501") deterministic
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Build a three-domain graph with explicit inference evidence and conflict reporting.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct evidence-based inference, graph boundaries, adapters, uncertainty, and conflict handling?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 13: Differentiable Simulation

## Learning objectives

- Explain the role of gradient paths, solver state, stability, integrator identity, and replayable derivatives in the DeepML Specialized evidence chain.
- Author and inspect a bounded differentiable simulation program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Differentiable Simulation is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **gradient paths, solver state, stability, integrator identity, and replayable derivatives**. Exposes simulation dynamics to gradient-based reasoning while retaining integrator, stability, causality, and replay evidence. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_02504
policy deterministic
policy no_network
domain hybrid_2 {
  import physics as P
  import finance as F
  import robotics as R
  graph DomainGraph02504 {
    state = P.differentiable_simulation(sensor_stream(provenance=sha256("2504")))
    risk = F.risk_model(state, horizon=15d)
    control = R.sensor_fusion(state, risk)
    output = domain_infer(control)
  }
  custom kernel HybridKernel hash sha256("kernel:02504") deterministic
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Specify a differentiable simulation with bounded gradient and stability checks.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct gradient paths, solver state, stability, integrator identity, and replayable derivatives?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 14: Risk–Physics Coupling

## Learning objectives

- Explain the role of physical state, financial or operational risk, uncertainty, judgement, and non-collapse rules in the DeepML Specialized evidence chain.
- Author and inspect a bounded risk physics coupling program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Risk–Physics Coupling is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **physical state, financial or operational risk, uncertainty, judgement, and non-collapse rules**. Connects physical state and risk state without silently conflating units, causality, uncertainty, or judgement. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_02503
policy deterministic
policy no_network
domain hybrid_1 {
  import physics as P
  import finance as F
  import robotics as R
  graph DomainGraph02503 {
    state = P.differentiable_simulation(sensor_stream(provenance=sha256("2503")))
    risk = F.risk_model(state, horizon=14d)
    control = R.sensor_fusion(state, risk)
    output = domain_infer(control)
  }
  custom kernel HybridKernel hash sha256("kernel:02503") deterministic
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Couple a physical state to a risk estimate without merging units or causal roles.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct physical state, financial or operational risk, uncertainty, judgement, and non-collapse rules?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 15: Calibration and Constraint Systems

## Learning objectives

- Explain the role of objectives, calibration ranges, constraints, tolerances, uncertainty, and invalid-state handling in the DeepML Specialized evidence chain.
- Author and inspect a bounded calibration program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Calibration and Constraint Systems is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **objectives, calibration ranges, constraints, tolerances, uncertainty, and invalid-state handling**. Associates observations and models through a versioned calibration state, objective, tolerance, uncertainty, and evidence record. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_01003
policy deterministic
policy no_network
domain graphics {
  unit InputUnit = base("input")
  tensor x: f64<InputUnit>[1,4]
  operator calibrate(x) -> Tensor pure deterministic
  calibration C01003 { method: bounded_least_squares tolerance: 1e-6 }
  constraint PhysicalBounds { min: 0 max: 203 }
  validate x with [calibrate, C01003, PhysicalBounds]
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Create a calibration profile and test unstable and contradictory conditions.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct objectives, calibration ranges, constraints, tolerances, uncertainty, and invalid-state handling?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 16: Sparse Planning and Kernel Selection

## Learning objectives

- Explain the role of dependency graphs, capability matching, deterministic implementation choice, and execution plans in the DeepML Specialized evidence chain.
- Author and inspect a bounded sparse planning program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Sparse Planning and Kernel Selection is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **dependency graphs, capability matching, deterministic implementation choice, and execution plans**. Builds an efficient execution plan for sparse graphs while preserving dependencies, determinism, and evidence. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_07539
policy deterministic
policy no_network
domain optimized_4 {
  unit meter = base("length")
  unit second = base("time")
  tensor velocity: f64<meter/second>[9,6]
  graph DomainGraph07539 { a = velocity * 1 b = sparse(a) c = calibrated(b, constant=1.0) }
  optimize DomainGraph07539 using [unit_propagation, dimensional_simplification, op_specialization, sparse_planning, calibration_folding, target_lowering]
  lower DomainGraph07539 to DEEPML_SPECIALIZED_R12
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Compare two kernels and publish the deterministic selection proof.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct dependency graphs, capability matching, deterministic implementation choice, and execution plans?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 17: Specialization, Folding, and Dimensional Simplification

## Learning objectives

- Explain the role of equivalence-preserving compiler transformations and their evidence obligations in the DeepML Specialized evidence chain.
- Author and inspect a bounded op specialization program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Specialization, Folding, and Dimensional Simplification is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **equivalence-preserving compiler transformations and their evidence obligations**. Specializes a generic operator for a domain, type, shape, or target without changing its declared meaning. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_07505
policy deterministic
policy no_network
domain optimized_0 {
  unit meter = base("length")
  unit second = base("time")
  tensor velocity: f64<meter/second>[9,5]
  graph DomainGraph07505 { a = velocity * 1 b = sparse(a) c = calibrated(b, constant=1.0) }
  optimize DomainGraph07505 using [unit_propagation, dimensional_simplification, op_specialization, sparse_planning, calibration_folding, target_lowering]
  lower DomainGraph07505 to DEEPML_SPECIALIZED_R12
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Apply one specialization and one calibration fold with exact equivalence evidence.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct equivalence-preserving compiler transformations and their evidence obligations?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 18: Target Lowering and R12/MCRT Emission

## Learning objectives

- Explain the role of stable relations, operators, hashes, status, confidence, provenance, and downstream identity in the DeepML Specialized evidence chain.
- Author and inspect a bounded r12 mcrt lowering program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Target Lowering and R12/MCRT Emission is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **stable relations, operators, hashes, status, confidence, provenance, and downstream identity**. Emits stable relations, operators, confidence, status, provenance, and replay identities for downstream JA21 layers. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_07502
policy deterministic
policy no_network
domain optimized_2 {
  unit meter = base("length")
  unit second = base("time")
  tensor velocity: f64<meter/second>[6,2]
  graph DomainGraph07502 { a = velocity * 1 b = sparse(a) c = calibrated(b, constant=1.0) }
  optimize DomainGraph07502 using [unit_propagation, dimensional_simplification, op_specialization, sparse_planning, calibration_folding, target_lowering]
  lower DomainGraph07502 to DEEPML_SPECIALIZED_R12
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Lower a domain graph and verify that every source relation has a stable emitted identity.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct stable relations, operators, hashes, status, confidence, provenance, and downstream identity?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 19: Hybrid Packages and Integrated Domain Stacks

## Learning objectives

- Explain the role of scientific, financial, simulation, graphics, and robotics composition under one policy envelope in the DeepML Specialized evidence chain.
- Author and inspect a bounded hybrid domain package program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Hybrid Packages and Integrated Domain Stacks is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **scientific, financial, simulation, graphics, and robotics composition under one policy envelope**. Publishes a cross-domain graph and its adapters, policies, dependencies, and evidence as one bounded artifact. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_05003
policy deterministic
policy no_network
domain workflow_5 {
  graph DomainGraph05003 {
    science = scientific_pipeline(dataset="local:05003")
    portfolio = portfolio_risk(science, currency=USD)
    simulation = simulation_environment(portfolio, steps=603)
    graphics = graphics_pipeline(simulation)
    robot = robotics_control(graphics, actuation=declaration_only)
  }
  package hybrid DomainGraph05003 as "hybrid_05003.msslb"
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Package an integrated local workflow with explicit adapters, dependencies, and limitations.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct scientific, financial, simulation, graphics, and robotics composition under one policy envelope?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 20: Safety Diagnostics and Certification

## Learning objectives

- Explain the role of network, actuation, units, constraints, calibration, causality, and hash rejection in the DeepML Specialized evidence chain.
- Author and inspect a bounded unsafe actuation program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Safety Diagnostics and Certification is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **network, actuation, units, constraints, calibration, causality, and hash rejection**. Certification case requiring rejection of undeclared or unauthorized physical actuation. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_00001
policy deterministic
policy no_network
domain finance {
  unit U1 = base("finance")
  schema Sample00001 { value: f64<U1> timestamp: Time provenance: Hash }
  tensor observations: f64<U1>[2,3]
  operator normalize_finance(x: Tensor<U1>) -> Tensor<Dimensionless> pure
  adapter SampleToTensor from Sample00001 to Tensor<U1>
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Run a stage-aware safety campaign and compare ordinary diagnostics with holdouts.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct network, actuation, units, constraints, calibration, causality, and hash rejection?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 21: Smithson 8S Coupled Mechanics Profile

## Learning objectives

- Explain the role of latent geometry, elucidation, phase, coupling, projection, judgement, uncertainty, and claim boundaries in the DeepML Specialized evidence chain.
- Author and inspect a bounded provenance kernel program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Smithson 8S Coupled Mechanics Profile is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **latent geometry, elucidation, phase, coupling, projection, judgement, uncertainty, and claim boundaries**. Makes origin, transformation history, hashes, and evidence propagation part of the executable semantics. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_02506
policy deterministic
policy no_network
domain hybrid_4 {
  import physics as P
  import finance as F
  import robotics as R
  graph DomainGraph02506 {
    state = P.differentiable_simulation(sensor_stream(provenance=sha256("2506")))
    risk = F.risk_model(state, horizon=17d)
    control = R.sensor_fusion(state, risk)
    output = domain_infer(control)
  }
  custom kernel HybridKernel hash sha256("kernel:02506") deterministic
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Map one specialized graph to an 8S evidence record without presenting the profile as established physics.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct latent geometry, elucidation, phase, coupling, projection, judgement, uncertainty, and claim boundaries?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Chapter 22: Standalone Compiler and Runtime Capstone

## Learning objectives

- Explain the role of a bounded implementation plan from parser to local replay, conformance, publication, and release evidence in the DeepML Specialized evidence chain.
- Author and inspect a bounded target lowering program.
- Identify the earliest responsible compiler or runtime failure stage.
- Preserve deterministic, no-network, provenance, unit, and R12/MCRT requirements.
- Design positive, diagnostic, and certification tests for the chapter invariant.

## Core lesson

Standalone Compiler and Runtime Capstone is taught as a chain of accountable transformations rather than as isolated syntax. The source program declares a language version, a module identity, deterministic and no-network policies, and a domain boundary. Parsing produces a stable AST. Name resolution connects imports and declarations. Type and unit checking establish whether shapes, schemas, dimensions, and adapters can compose. Semantic validation determines whether the declared operation means what its operator profile says it means. Safety gates constrain network access, unknown code, market connectivity, physical actuation, and other capabilities. Only then may normalization, optimization, R12 lowering, MCRT emission, and bounded runtime admission proceed.

The central focus of this chapter is **a bounded implementation plan from parser to local replay, conformance, publication, and release evidence**. Maps specialized semantics into a declared backend representation while preserving units, policies, hashes, and provenance. A trustworthy implementation records not only the final value but also the identities and assumptions that make the value interpretable: source hash, semantic hash, module and domain IDs, unit and shape information, calibration version, constraint set, provenance, operator or kernel hash, deterministic seed, expected stage, diagnostic behavior, R12 relation, MCRT relation, runtime trace, and stated limitations. These fields make it possible to compare two runs without pretending that equal-looking results prove equal semantics.

Specialized programming is difficult because each domain brings its own vocabulary and failure modes. A financial horizon is not a simulation timestep. A graphics coordinate is not automatically a robotic frame. A confidence score is not a physical unit. A rendered overlap is not a latent geometric collision. An adapter that silently drops provenance or converts units without a declared rule may produce convenient output while corrupting meaning. Therefore the language requires explicit boundaries and makes cross-domain composition a governed operation.

The review council applies five complementary lenses. SOPHIA checks mathematical precision, dimensions, assumptions, and claim limits. CHARLOTTE checks names, taxonomy, discoverability, and whether two domains are being described consistently. LANDON checks compiler stages, runtime policy, deterministic replay, diagnostics, packaging, and integrity evidence. Professor converts the concept into a progression of explanation, exercise, failure analysis, and assessment. Podium makes the suite readable and navigable so that technical evidence can be found instead of hidden in a large archive.

A positive record passes only when its complete contract remains intact. A diagnostic record passes when it is rejected at the earliest responsible stage with the expected diagnostic. A certification holdout passes when a frozen implementation demonstrates the required rejection without special-casing the answer. This distinction prevents a common testing error: treating any program that reaches runtime as successful. In a safety-oriented language, correct refusal is often the required result.

The practical goal is not to make every domain identical. It is to give each domain a strong local type and evidence model while providing explicit adapters for valid cooperation. When this principle is followed, finance, science, graphics, robotics, and simulation can share a graph without losing their separate units, authorities, clocks, uncertainties, and provenance. When it is violated, the graph becomes an attractive but uninterpretable collection of calculations.

## Corpus-derived program

```deepml
deepml specialized 0.3
module corpus.deepml_specialized.example_07501
policy deterministic
policy no_network
domain optimized_1 {
  unit meter = base("length")
  unit second = base("time")
  tensor velocity: f64<meter/second>[5,12]
  graph DomainGraph07501 { a = velocity * 1 b = sparse(a) c = calibrated(b, constant=1.0) }
  optimize DomainGraph07501 using [unit_propagation, dimensional_simplification, op_specialization, sparse_planning, calibration_folding, target_lowering]
  lower DomainGraph07501 to DEEPML_SPECIALIZED_R12
}
```

## Program reading guide

1. Identify the domain, imports, policies, schemas, units, tensors, operators, adapters, graph, and package declarations.
2. State the semantic operator and the expected compiler or runtime stage.
3. List every assumption that is not encoded directly in the source.
4. Separate local deterministic evidence from external systems or device effects.
5. Locate the source hash, semantic hash, R12 relation, MCRT relation, and validation result in the corpus record.

## Engineering checklist

- Preserve language, module, domain, schema, operator, package, and relation identities.
- Declare units, shapes, timestamps, frames, horizons, clocks, calibration, constraints, and uncertainty.
- Enforce deterministic and no-network policy through compiler and runtime evidence.
- Keep market access, physical actuation, unknown code, and external devices behind explicit capabilities.
- Reject invalid structure or semantics at the earliest responsible stage.
- Preserve source hash, semantic hash, operator hash, R12 relation, MCRT relation, provenance, and replay context.
- Distinguish exact identity, numerical tolerance, visual similarity, and judgement equivalence.

## Laboratory

Publish a versioned toolchain plan and execute every structural validator supplied by the suite.

## Evidence to submit

- Selected corpus and script IDs
- Source and semantic hashes
- Expected compiler/runtime stage and result
- Units, shapes, adapters, calibration, and constraint profile
- Diagnostic, operator, or kernel identity
- R12/MCRT fields affected
- Replay inputs, output evidence, uncertainty, authority boundary, and limitations

## Review questions

1. What invariant defines correct a bounded implementation plan from parser to local replay, conformance, publication, and release evidence?
2. Which compiler or runtime stage should establish or reject that invariant?
3. Which units, clocks, frames, horizons, or calibration states must remain explicit?
4. How could plausible output conceal a semantic, safety, or provenance defect?
5. Which positive, diagnostic, and certification cases provide adequate coverage?

---

# Appendix A: Corpus Profile

- Records: 10,000
- Topics: 42
- Positive: 7,875
- Ordinary diagnostics: 1,125
- Certification holdouts: 1,000
- Tiers: 1 (1,000), 2 (1,500), 3 (2,500), 4 (2,500), 5 (1,500), 6 (1,000)

# Appendix B: Required Standalone Policies

- Deterministic evaluation
- No network access
- No unknown code execution
- Stable domain, schema, operator, package, and relation identifiers
- Provenance preservation
- Explicit unit, shape, clock, horizon, calibration, constraint, equivalence, and tolerance profiles
- External market and physical actuation forbidden unless separately authorized
- Rejection at the earliest responsible stage

# Appendix C: Native-Evidence Boundary

The textbook and suite describe a source-to-runtime contract derived from the uploaded corpus. Native compilation, scientific computation, portfolio analysis, graphics rendering, robotic execution, simulation, and replay remain implementation tasks until a conforming compiler and runtime are supplied and tested.
