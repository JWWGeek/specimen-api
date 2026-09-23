# Decision log

## 001 – Branching strategy

**Date:** 2026-09-23
**Status:** Accepted

**Context:** Solo learning project that should mirror team practices.

**Decision:** Simplified Git Flow: `main` (production), `develop` (integration),
short-lived `feature/*` branches. All changes reach `main` and `develop` via pull
request, enforced by a GitHub ruleset.

**Alternatives considered:** Trunk-based development. Simpler and faster, but
relies on mature automated testing, which this project doesn't have yet.

**Consequences:** Slightly more overhead per change; clear separation between
tested and in-progress work.
