
# Specialized Language Domain Architecture

```text
Local data and declared provenance
        │
        ▼
Schemas ── Units ── Domain tensors
        │             │
        ├── Adapters ─┤
        ▼             ▼
Domain operators and custom kernels
        │
        ▼
Typed multidomain graph
        │
        ├── calibration / constraints / uncertainty
        ├── no-network / authority / deterministic gates
        ├── optimization with equivalence evidence
        ▼
R12 lowering ── MCRT emission ── bounded runtime replay
```

Rendering, financial estimates, simulation output, and robotic declarations are observations or products of the graph. They do not replace unit, provenance, causal, safety, or judgement evidence.
