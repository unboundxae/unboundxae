# Shaw

**Product and operations builder working with AI-assisted software development.**

I turn operational problems into explicit requirements, testable components, and decisions people can review. My focus is the workflow: what context matters, where human judgment belongs, and how a system should behave when evidence is missing.

## Selected work

| Project | Problem and work | Status |
| --- | --- | --- |
| [KAIA HIVE — Community Agent](docs/community-agent.md) | An intended workbench for reviewing audience comments in context and preparing selective reply drafts. The retained engineering work covers review gates, SQLite persistence and recovery, reporting, and consistency checks. | Reviewed synthetic components; end-to-end production use is not established. |
| [Swarm Manifest Pilot](docs/manifest-pilot.md) | A small Python metadata validator built by two AI workers, independently checked by another agent, then integrated in sequence. The pilot also exercised conflict, stale-update, and duplicate-delivery controls. | Completed synthetic pilot; production adoption is separate. |

## My contribution

I own the product direction, requirements, acceptance decisions, and consequential approvals. I use AI agents for implementation and review, and direct corrections when results do not meet the agreed scope. These projects represent that collaboration; I do not claim to have manually written every file.

The work demonstrates workflow design, explicit interfaces, adversarial evaluation, failure handling, and traceable decisions. The examples use **Python, SQLite, JSON/JSON Schema, and Git**.

## How I work

1. Define the problem, boundaries, and acceptance criteria.
2. Give implementation and review separate responsibilities.
3. Check exact versions; retain failures, corrections, and limitations.
4. Keep a passing test separate from permission to release or act.

The case studies describe evidence available on **October 22, 2026**. Source repositories remain private; these summaries do not provide public reproduction of the underlying tests. See the [portfolio scope](docs/portfolio-scope.md) for how claims and updates are handled.
