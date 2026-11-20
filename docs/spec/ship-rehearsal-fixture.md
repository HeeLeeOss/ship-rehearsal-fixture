---
title: Ship rehearsal fixture
license: CC0-1.0
lifecycle: ai-full
---

## Problem

The `ship` stage of the full-SDLC lane has never run against a real keyring, a real Zenodo answer or a real GitHub pull request. Its tests use fakes, so nobody yet knows what a real run does or where it stops. The Hee-Lee Oss maintainers need to see one run end to end before any real publication.

## Beneficiary

The Hee-Lee Oss maintainers. This is an internal rehearsal with no outside beneficiary. The output is a pair of tiny text files and a record of what happened, reached through this repository and Zenodo's sandbox, whose DOIs do not resolve.

## Scope

Two text files, one per milestone: `data/m1.txt` for milestone M1 and `data/m2.txt` for milestone M2. Each milestone is then read, covered and shipped to Zenodo's sandbox on its own, so that one run can be uninterrupted and another can be killed and resumed.

## Non-goals

No real publication, no production DOI, no software and no content that anyone is meant to use. Nothing in this project is delivered to anyone.

## Acceptance criteria

| AC | Case | Required evidence |
|---|---|---|
| AC-01 | `data/m1.txt` holds the line "rehearsal one" | The file at the tip of the default branch |
| AC-02 | `data/m2.txt` holds the line "rehearsal two" | The file at the tip of the default branch |

## Inputs and provenance

None
