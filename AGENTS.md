# BINDING SCIENTIFIC GOVERNANCE

Authoritative source for the scientific thesis framing:
`01_GOVERNANCE/Bachelorarbeit-THEMA.txt`.

1. Exactly three subordinate research questions exist: FF1-FF3.
2. Never introduce FF4.
3. Cascade is a prototype/system-artifact extension, not a research question.
4. Active Learning is exploratory and not Self-Supervised Learning.
5. Core thesis conclusions must be derived from FF1-FF3.
6. Experimental evidence hierarchy must be respected.
7. Historical/pilot results must not override final N10 evidence.
8. Never invent missing experimental evidence.
9. Every quantitative thesis claim must be traceable to:
   Experiment -> canonical notebook -> output file -> filter -> value.
10. Do not modify scientific result files unless explicitly instructed.

## Research Question Freeze

Main research question:

Wie beeinflusst Self-Supervised Representation Learning die
Generalisierungsfaehigkeit von Verfahren zur automatisierten Erkennung bisher
ungesehener Phishing-Webseiten?

FF1:
Wie unterscheiden sich selbstueberwacht erlernte und nicht zusaetzlich
selbstueberwacht angepasste Repraesentationen hinsichtlich ihrer Eignung fuer
die Phishing-Klassifikation?

FF2:
Wie veraendert sich der Nutzen selbstueberwacht erlernter Repraesentationen
unter zeitlichem und strukturellem Distribution Shift?

FF3:
Wie veraendert sich der Nutzen selbstueberwacht erlernter Repraesentationen
bei unterschiedlicher Verfuegbarkeit gelabelter Trainingsdaten?

There is no FF4, RQ4, cascade research question, triage research question, or
Active-Learning research question in the final thesis framing.

## Prototype And Extensions

The selective cascade is a prototypische Anwendung bzw. Erweiterung des
Software-Artefakts. It operationalizes findings from the empirical core in a
system-oriented prototype. Review-assisted recall is an assisted upper-bound
metric and must not be conflated with automatic Stage-1 FPR or with proof that
SSL itself works.

Active Learning is a possible downstream extension of the software artifact.
It is exploratory, not SSL, and not required to succeed for FF1-FF3 or the main
research question to be answered.

## Evidence Hierarchy

1. E03 FINAL N10: primary system, shift, low-FPR, and cascade evidence.
2. E01 Core Freeze: primary controlled representation evidence.
3. E04 Productive AL: exploratory Active-Learning extension.
4. E06 ALxSSL Original10: exploratory interaction analysis.
5. E07 Independent Replication10: independent replication once complete.
6. E05 SSL Refresh: supporting ablation.
7. E02 Hybrid 5-Seed: support/provenance where not superseded by N10.

Historical notebooks under `03_NOTEBOOK_HISTORY/` and legacy outputs under
`99_LEGACY_PROVENANCE_ONLY/` must never become final evidence.
