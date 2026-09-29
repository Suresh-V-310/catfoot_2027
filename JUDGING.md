# JUDGING

## Assignment
The MVP supports seeded judge assignment. The data model keeps assigned submission IDs per judge.

## Rubric
Innovation: 25%
Technical: 35%
Impact: 25%
Design: 15%

## Normalization
Each judge score is converted to a 0-10 average. The submission's displayed normalized score is the mean across its assigned judge scores.

## Integrity
The production architecture must enforce judge/organizer/participant permissions server-side, prevent a judge from modifying another judge's scores, and retain an immutable audit trail.
