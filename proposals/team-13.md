# DSAN 6725 Final Project Proposal

## Team Number

13

## Team Name

Roomwise

## Team Members

| Name | NetID |
| ---- | ----- |
| Samuel Villarreal | sv635 |
| Junyi Tang | dt786 |
| Juncheng Han | jh2732 |
| Tianyu Zhao | tz297 |

## Project Title

Roomwise: An AI Agent for Roommate Matching and Apartment Search

## Abstract

Renters must balance housing costs, commute times, amenities, and roommate compatibility across incomplete listings. Roomwise will help Washington, DC renters compare apartments, with optional roommate matching for two-person households, and understand costs and trade-offs.

A coordinator will collect budgets, move-in dates, locations, transportation needs, and living preferences. It will pass structured profiles to a matching agent that ranks consenting users and explains compatibility conflicts. A search agent will retrieve apartments for individuals or proposed pairs, using RentCast listings, permitted property websites for amenities and fees, and Google Routes and Places for commutes and nearby facilities. A verification agent will reconcile property and unit identities, flag conflicting evidence, and calculate known costs before the coordinator returns ranked recommendations with source citations. Unknown fees will remain explicit; users must approve contact sharing. API access and website permissions remain to be verified before implementation.

We propose running the agents on a local Linux VM using hosted Claude Sonnet 4.5 for tool use and structured extraction, with deterministic code for scoring and arithmetic. Each completed search will be measured for median and p95 latency, API and model cost, and throughput.

Evaluation will use 100 held-out synthetic renter scenarios and consented profiles when available. Two teammates will label eligible apartments, amenities, and costs from dated source snapshots, resolving disagreements. Against deterministic apartment filters and preference-based roommate scoring on the same cases, we target at least 95% hard-constraint satisfaction, 90% amenity extraction F1, and lower cost-calculation error. Blinded participant preferences will assess ranking usefulness; reported rates will include sample sizes and confidence intervals.

The biggest eight-week risk is inaccessible or incomplete rental data. We will test access first and fall back to a permitted, manually curated DC listing dataset with dated evidence, limiting claims about live availability.
