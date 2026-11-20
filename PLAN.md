---
title: Ship rehearsal fixture
riskTier: low
license: CC0-1.0
lifecycle: ai-full
beneficiary: Hee-Lee Oss maintainers (a ship rehearsal fixture; no public deliverable)
definitionOfShipped: A Zenodo sandbox rehearsal deposit per milestone; nothing is delivered to anyone.
reviewPolicy:
  humanCheckpoints: [spec, plan, ship]
milestones:
  - { id: M1, title: Rehearsal one, rows: [AC-01] }
  - { id: M2, title: Rehearsal two, rows: [AC-02] }
definitionOfShippedRecipe:
  kind: zenodo-deposit
  params:
    paths: [data/]
    environment: sandbox
    metadata:
      title: Hee-Lee Oss ship rehearsal fixture
      description: A sandbox rehearsal of the ship stage. Not a real publication.
      creators: [{ name: "Hee-Lee Oss" }]
      uploadType: dataset
---

## Summary

A throwaway project that exists once, to rehearse the `ship` stage of the full-SDLC lane against Zenodo's sandbox. It holds two tiny text files, one per milestone, so each milestone can be read, covered and shipped on its own. It is a good deed only in that it proves the ship path before any real publication; it has no outside beneficiary.

## Scope

In scope: `data/m1.txt` for milestone M1 and `data/m2.txt` for milestone M2, and one sandbox deposit per milestone. Out of scope: any real publication, any production DOI, and any content anyone is meant to use.

## Risk

Low. There is no personal data, no high-stakes advice, no outside beneficiary and no real deliverable. The licence is CC0-1.0 and the project's only inputs are two lines of text written for the rehearsal. It carries no evaluators, because the sandbox half of the shipped-tree evaluation is not built, and a project that needs one cannot ship yet.

## Approach

The maintainer writes each file by hand on the donated lane and merges its pull request. Each milestone then has one real coverage read, whose record is merged by a person. `hee-lee-oss ship` is run at a terminal for each milestone, with a person typing the plan's digest. The first milestone is shipped without interruption. The second is killed after the draft is created and again after it is published, and is run again each time.

## Definition of shipped

A sandbox deposit exists for the milestone, its bytes fetched back from Zenodo match the bytes in the repository, and `SHIPPED.md` records it as a rehearsal. Nothing is delivered to anyone, and the sandbox DOIs do not resolve.
