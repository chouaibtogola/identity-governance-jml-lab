# Identity Governance Lab — Joiner-Mover-Leaver (JML)

A hands-on lab demonstrating identity lifecycle governance in Microsoft Entra ID, built on the same fictional company and tenant as the [Zero-Trust IAM Lab](https://github.com/chouaibtogola/zero-trust-iam-lab).

Where the Zero-Trust IAM Lab controls **how** someone signs in, this lab controls **whether their access reflects who they currently are** throughout the identity lifecycle. It demonstrates how identity governance can reduce access drift, automate onboarding and offboarding, and prevent unnecessary access from remaining active after a user's role or employment status changes.

## Why this project

Conditional Access controls access based on conditions such as user risk, location, device state, and authentication strength, but it does not manage the full employee identity lifecycle.

JML governance addresses what happens when a user **joins, changes roles, or leaves** an organization. Automating these lifecycle events reduces manual onboarding and offboarding errors, limits access drift, and helps prevent orphaned accounts or unnecessary access from remaining active after a user's role changes.

## What's implemented

| Area | Status |
|---|---|
| Dynamic membership groups (attribute-based) | ✅ |
| Lifecycle Workflow — Joiner (onboarding) | ✅ |
| Lifecycle Workflow — Leaver (offboarding) | ✅ |
| Access packages & entitlement management | ⏳ |
| Access review / certification on the access package | ⏳ |

## Repo structure

```text
/policies/       Exported JSON/config of dynamic groups, workflows, access packages
/workflows/      Lifecycle Workflow definitions and run logs
/scenarios/      Test scenario write-ups with screenshots — the actual proof
/diagrams/       JML flow diagrams
/screenshots/    Supporting screenshots referenced by /scenarios