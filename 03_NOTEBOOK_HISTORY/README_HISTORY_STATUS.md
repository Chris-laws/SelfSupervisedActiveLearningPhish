# Notebook-Historie / Fehlerstatus

Diese Dateien werden **aufbewahrt**, aber nicht als kanonische Berechnungsquelle verwendet.

## Core Freeze
- `phreshphish_final_freeze_evaluation.ipynb` – v1
- `..._v2.ipynb` – Loader-Hotfix
- `..._v3.ipynb` – 40k-aware OOD-Rekonstruktion
- `..._v4.ipynb` – finalisierte 40k-aware Szenariogrößen, später Xtrain-Scope-Bug
- `..._v5_resume.ipynb` – **kanonisch**, behebt Xtrain-Scope-Bug + Resume

## Hybrid
- `...fpr_apfix.ipynb` – ältere Fassung
- `...v3_resume.ipynb` – **kanonischer 5-Seed-Support**
- `FINAL_BACHELOR_RUN.ipynb` – 5-Seed-Gesamtlauf, durch N10 ersetzt

## Productive AL
- `PRODUCTIVE_CASCADE_AL_SSL_LOOP.ipynb` – **kanonisch für AL**; teurer Loop lief durch,
  Fehler trat erst beim optionalen SSL-Refresh auf.
- `...v2_RESUME_FIX.ipynb` – Resume-Versuch; erkannte Input, aber rechnete teure Loop-States neu;
  **nicht kanonisch**.

## SSL Refresh
- `FINISH_ONLY.ipynb` – Preflight scheiterte wegen angenommener Unterordnerstruktur.
- `FINISH_ONLY_v2_FLAT_KAGGLE.ipynb` – **kanonisch**, Complete.

## AL×SSL Original10
- `OVERNIGHT.ipynb` – geplante Vollversion, nicht finale Ausführung.
- `FAST_3H30.ipynb` – Preflight scheiterte an Budget-Key-Serialisierung.
- `FAST_3H30_v2_BUDGETKEY_FIX.ipynb` – **kanonisch**, Complete.

## Cascade Error Notebook
- `cascade_error_analysis_25pct.ipynb` ist als Support-Historie erhalten.
- Seine eigenständigen Originaloutputs sind lokal nicht vollständig nachgewiesen.
- Keine daraus stammende Zahl als einzige Evidenz verwenden, solange Originaloutputs fehlen.
