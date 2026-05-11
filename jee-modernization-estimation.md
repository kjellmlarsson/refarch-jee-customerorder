You are estimating an AI-assisted Java modernization project.

Use a modernization spiderweb, not a single score.

Assess these six dimensions:

1. Structural scope
   - modules, repositories, source roots, generated code, build files,
     deployment files, API contracts, shared libraries, ownership boundaries

2. Semantic complexity
   - framework behavior, persistence, security, transactions, reflection,
     classloading, generated code, app-server-specific APIs, serialization,
     concurrency, schedulers

3. Knowledge transparency
   - documentation, ADRs, internal frameworks, blueprints, conventions,
     code generators, examples, runbooks, ownership, known tribal knowledge gaps

4. Integration and data surface
   - APIs, queues, files, schemas, database contracts, partner formats,
     data type mappings, data conversion, downstream consumers, upstream producers

5. Feedback readiness
   - local build, CI health, test reliability, contract tests, integration
     environments, test data, observability, acceptance criteria

6. Operational and governance constraints
   - security, compliance, audit, release windows, change approval,
     production access, rollback, support ownership, SLOs

Also estimate:

7. Pass intensity
   - expected compile/test/repair loops per slice
   - expected human clarification points
   - likely causes of rework

8. Token accounting regime
   - provider and model
   - input/output/cached/reasoning token categories
   - tool schemas and file inputs included
   - prompt caching assumptions
   - log truncation and context compaction strategy

Produce:

- measured signals
- inferred risks
- weak spiderweb spokes
- AI assessment suitability
- recommended deterministic tools before LLM work
- representative calibration slices
- P50 and P80 token budget ranges by phase
- the assumptions that would invalidate the estimate