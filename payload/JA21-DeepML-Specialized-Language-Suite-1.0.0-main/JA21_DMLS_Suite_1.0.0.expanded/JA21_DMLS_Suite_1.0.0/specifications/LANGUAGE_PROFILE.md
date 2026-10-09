
# DeepML Specialized Standalone Language Profile

## Identity

- Language: `deepml.specialized`
- Source language version: `0.3`
- Standalone suite version: `1.0.0`
- Default policies: deterministic, no network, no unknown code execution, stable IDs, provenance preservation

## Semantic pillars

1. **Domain identity:** every schema, tensor, operator, adapter, and package belongs to an explicit namespace.
2. **Dimensional integrity:** units and conversions are typed and checked rather than inferred from labels.
3. **Provenance:** source, calibration, transformation, and package history travel with the computation.
4. **Bounded authority:** network and physical actuation are separate capabilities and are forbidden by default.
5. **Cross-domain explicitness:** coupling requires named adapters, assumptions, uncertainty, and judgement boundaries.
6. **Deterministic evidence:** compilation, optimization, lowering, selection, and replay use stable rules and identities.
7. **Earliest-stage diagnostics:** invalid programs fail at the first responsible compiler or runtime validation stage.

## Native implementation boundary

This profile is reconstructed from the corpus and its source specifications. A conforming implementation must independently prove parsing, typing, policy enforcement, optimization equivalence, R12/MCRT emission, and runtime behavior.
