# Swarm Manifest Pilot

**A completed synthetic exercise in parallel implementation, independent agent review, and serial Git integration.**

Status as of October 22, 2026: the bounded pilot completed and was integrated into a private repository. It is separate from the wider PRIME SWARM program and does not establish that program's production readiness.

## Problem and delivered scope

Parallel AI workers need an agreed interface, clear ownership, and a way to reconcile changes before they reach the same target. This pilot exercised that workflow while producing a small metadata validator for possible future tooling.

The Python standard-library validator accepts a UTF-8 JSON document of at most 65,536 bytes with exactly four string fields: a synthetic scene ID, prompt version, asset-digest string, and review state. It checks field rules and rejects malformed inputs, duplicate keys, extra fields, invalid encoding, excessive nesting, and oversized documents. Its command-line output and exit codes are deterministic. A JSON Schema describes the parsed-object constraints.

The digest check validates the string's format; it does not hash or verify an asset. An `approved` value is data, not permission to act.

## My contribution and AI assistance

I authorized the bounded task and its publication scope. Two AI workers implemented separate responsibilities: one built the schema and validator; the other built fixtures, a test runner, and usage examples. A separate agent reviewed the frozen candidates. The coordinating agent handled integration and recorded the results under my authorization.

Both workers started from a pinned base and owned separate paths. The coordinator integrated the first change, had the second checked against the changed target, then integrated it. A disposable local drill exercised conflicts, stale updates, concurrent integration attempts, interruption recovery, and duplicate delivery.

## Recorded evaluation

| Evaluation scope | Recorded result |
| --- | --- |
| Product fixture runner | 77/77 passed: 73 fixtures and four command-line probes. |
| Independent agent review of the exact candidate after the target changed | 1,022/1,022 checks passed with the unchanged harness in private temporary storage. |
| Coordinator's disposable local control drill | 8/8 checks passed; the reviewer inspected its source and evidence but did not independently execute the merges. |

These are results from named synthetic test scopes, not production coverage percentages. The source, harnesses, and detailed records remain private; readers cannot reproduce these results from this summary alone.

The changed-target review initially stopped integration when cleanup observations conflicted. Subsequent evidence showed files being recreated after the candidate processes exited in the shared workspace. The restoring service was not identified. The unchanged harness passed in private temporary storage with its cleanup checks retained. No product change or relaxed check was used to obtain that pass.

## Results and limitations

The pilot demonstrates separate worker responsibilities, review bound to exact content, and sequential integration with a recheck when the target changes. Recorded GitHub integration was verified through coordinator browser observations and normalized text comparisons, not an independent remote Git-object audit.

Review was by another AI agent, not a separate human or certification body. Workers shared a runtime; their separation was procedural. Python 3.12.14 was exercised; Python 3.11 execution and full JSON Schema-engine conformance were not tested.

The validator does not check media existence, actual asset hashes, reviewer authority, content quality, or rights. No production queue, webhook, deployment, general exactly-once guarantee, or measured speedup follows. Future adoption needs its own scope and acceptance.

[Back to profile](../README.md) · [Portfolio scope](portfolio-scope.md)
