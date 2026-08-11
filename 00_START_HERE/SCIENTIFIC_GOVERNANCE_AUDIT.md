# Scientific Governance Audit

## Authoritative Source

The authoritative conceptual freeze is
`01_GOVERNANCE/Bachelorarbeit-THEMA.txt`. It was used as the highest-priority
source for the repository governance correction. Its scientific content was not
rewritten.

## Binding Research Questions

Main research question:

Wie beeinflusst Self-Supervised Representation Learning die
Generalisierungsfähigkeit von Verfahren zur automatisierten Erkennung bisher
ungesehener Phishing-Webseiten?

FF1:

Wie unterscheiden sich selbstüberwacht erlernte und nicht zusätzlich
selbstüberwacht angepasste Repräsentationen hinsichtlich ihrer Eignung für die
Phishing-Klassifikation?

FF2:

Wie verändert sich der Nutzen selbstüberwacht erlernter Repräsentationen unter
zeitlichem und strukturellem Distribution Shift?

FF3:

Wie verändert sich der Nutzen selbstüberwacht erlernter Repräsentationen bei
unterschiedlicher Verfügbarkeit gelabelter Trainingsdaten?

Confirmation: no FF4 exists in the final thesis framing. There is no cascade,
triage, system-design, or Active-Learning research question.

## FF4 Terminology Audit

Search terms:
`FF4`, `F4`, `Forschungsfrage 4`, `research question 4`, `RQ4`,
`triage research question`, `cascade research question`,
`active learning research question`.

### CURRENT_GOVERNANCE_WRONG

None found.

### HISTORICAL_PROVENANCE_KEEP

None found.

### FALSE_POSITIVE / unrelated

The following hits are not research-question terminology and were not changed:

- `90_UNASSIGNED_REVIEW/UNASSIGNED_FILES.csv:80` contains
  `TABLE01_primary_interaction_25pct_fpr005.csv`; this is a filename.
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/rescued_b0_false_negatives_seed42.csv`
  lines 4, 9, 33, 38, 51, 63, 68, and 231 contain the text fragment `F4` only
  inside hashes, URLs, or row text from preserved CSV evidence.
- `00_START_HERE/CURRENT_FILE_INVENTORY.csv` lines 8, 107, 138, and 150 contain
  `F4` only inside SHA256 hashes or filenames.
- `00_START_HERE/SECOND_PASS_RESOLVED_FILES.csv` lines 38, 39, 46, and 47
  contain `F4` only inside SHA256 hashes or paths.
- `00_START_HERE/FILE_HASHES_SHA256.csv` lines 83, 246, 257, 266, and 313
  contain `F4` only inside SHA256 hashes or manifest paths.
- `00_START_HERE/RESTRUCTURE_AUDIT.md` lines 115, 277, 287, 296, 329, 359,
  and 362 contain `F4` only inside SHA256 hashes or paths from the restructure
  audit.
- `00_START_HERE/RESTRUCTURE_AUDIT_V2.md` line 160 contains `F4` only inside a
  SHA256 hash for ZIP-contained evidence.

Corrective governance documents now intentionally state that no FF4 exists.
Those corrective statements are not classified as old FF4 terminology.

## Files Corrected

- `AGENTS.md`: created binding scientific governance for future agents.
- `00_START_HERE/README.md`: added the three-question framing and clarified
  that cascade and Active Learning are prototype/application extensions.
- `00_START_HERE/EVIDENCE_PRIORITY.md`: clarified that the evidence hierarchy
  serves FF1-FF3 and that cascade/AL are not research questions.
- `00_START_HERE/EXPERIMENT_REGISTER_AUDITED.csv`: clarified the E03/E04 roles
  without changing experiment evidence.
- `00_START_HERE/AUDIT_COMPLETENESS.md`: added a governance note for FF1-FF3
  and the non-FF role of cascade/AL.
- `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/README_INTERACTION.md`: clarified
  that ALxSSL interaction evidence is exploratory/supporting and not a
  research question.

## Historical Files Intentionally Left Unchanged

No historical FF4 wording was found. Historical notebooks and scientific result
artifacts were not modified.

## Role Of Cascade

The selective cascade is a prototypische Anwendung bzw. Erweiterung des
Software-Artefakts. It may include Stage 1 with `B0_STRUCT_XGB`, Stage 2 with
`T0_E2E` / `DAPT_E2E`, review budgets, rescue analysis, review precision,
review-assisted recall, comparison against B0 SELF ranking, and Stage-1
sensitivity/justification. These analyses are not independent research
questions.

Review-assisted recall is an assisted upper-bound metric. It must not be
conflated with automatic Stage-1 FPR, and cascade improvements must not be
presented as proof that SSL itself works.

## Role Of Active Learning

Active Learning is not Self-Supervised Learning. It is a possible downstream
extension of the software artifact and may be reported as exploratory,
prototype-lifecycle, application-oriented evidence. It does not prove FF1, FF2,
or FF3, and the ALxSSL interaction analysis is exploratory/supporting evidence.

## Current Evidence Hierarchy

1. E03 FINAL N10: primary system / shift / low-FPR / cascade evidence.
2. E01 Core Freeze: primary controlled representation evidence.
3. E04 Productive AL: exploratory Active-Learning extension.
4. E06 ALxSSL Original10: exploratory interaction analysis.
5. E07 Independent Replication10: independent replication once complete.
6. E05 SSL Refresh: supporting ablation.
7. E02 Hybrid 5-Seed: support/provenance where not superseded by N10.

Historical notebooks under `03_NOTEBOOK_HISTORY/` must never become final
evidence.

## Scientific Result Files

No notebook, CSV result value, JSON experiment result, model output, completion
marker, seed, metric, or experimental evidence file was modified for this
governance correction.

## git diff --stat

```text
00_START_HERE/AUDIT_COMPLETENESS.md                          |  6 ++++++
00_START_HERE/EVIDENCE_PRIORITY.md                           |  9 +++++++++
00_START_HERE/EXPERIMENT_REGISTER_AUDITED.csv                |  4 ++--
00_START_HERE/README.md                                      | 12 ++++++++++++
.../E06_AL_SSL_ORIGINAL10/EXTRACTED/README_INTERACTION.md    |  4 ++++
5 files changed, 33 insertions(+), 2 deletions(-)
```

Untracked governance files created in this correction:

- `AGENTS.md`
- `00_START_HERE/SCIENTIFIC_GOVERNANCE_AUDIT.md`
