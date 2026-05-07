
# AD ASTRA MCDO — STAGE3 PUBLIC SYNTHESIS

## Purpose

This package presents a public benchmark summary for a proprietary astronomical screening framework evaluated on labeled KOI benchmark data.

The public layer intentionally excludes internal scoring logic, feature weighting, routing rules, and implementation details.

The benchmark objective is not planet confirmation.

The benchmark objective is:
- workload reduction,
- false-positive reduction,
- structured routing,
- high-recall candidate preservation.

---

# Stage Summary

## Stage3A — KOI Labeled Benchmark

Result:
- Preliminary labeled benchmark completed.
- Public leak audit passed.

Observed operating profile:
- Recall target: 95%
- Measured recall mean: 0.9500
- Precision mean: 0.6624
- False-positive reduction mean: 0.5118
- Workload reduction mean: 0.2799

---

## Stage3B — Robustness Benchmark

Multiple randomized holdout variations were evaluated.

Observed result:
- Stable recall behavior across benchmark perturbations.
- Stable workload reduction behavior.
- Stable routing behavior.

The benchmark did not collapse under randomized splits.

---

## Stage3C — Noise / Anomaly Characterization

Reject streams were found to contain structured sub-groups rather than a single random noise population.

Observed public streams:
                        public_route  count  fraction
                   value-like stream   3830  0.416259
   signal-like false-positive stream   2303  0.250299
            anomaly-candidate stream   1445  0.157048
               typical reject stream    841  0.091403
       low-information reject stream    754  0.081948
value-labeled anomalous-shape stream     28  0.003043

Interpretation:
- Noise-like behavior is structured.
- Some streams exhibit signal-like geometry.
- Some rare anomalous structures remain value-labeled.

This suggests that reject-space analysis may itself contain information value.

---

## Stage3D — Data-Derived Visual Model

The included visualizations are generated directly from benchmark outputs.

They are:
- data-derived projections,
- not artistic illustrations,
- not astrophysical maps,
- not object confirmations.

Their purpose is to demonstrate:
- separability,
- routing structure,
- benchmark geometry,
- workload partitioning behavior.

---

# Important Limitations

This benchmark:
- does not confirm exoplanets,
- does not replace astrophysical validation,
- does not replace NASA vetting pipelines,
- does not claim physical discovery.

External validation remains required:
- centroid analysis,
- ephemeris matching,
- odd/even transit analysis,
- secondary eclipse checks,
- pixel-level vetting,
- literature verification.

---

# Conclusion

Observed benchmark evidence supports the claim that:
- structured screening may reduce downstream workload,
- high recall can be preserved simultaneously,
- reject-space is not purely random,
- benchmark routing behavior remains stable under perturbation.

This package is intended as:
- public evidence,
- partner review material,
- benchmark documentation.

It is not a final scientific publication.

