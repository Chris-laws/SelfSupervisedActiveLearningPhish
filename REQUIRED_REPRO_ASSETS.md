# EXTERNE REPRODUZIERBARKEITS-ARTEFAKTE – SEPARAT SICHERN

Der kleine `BA_MASTER_V2_AUDITED` ist das **Schreib-/Evidenzpaket**.
Für vollständige Reproduzierbarkeit müssen die GB-Artefakte daneben separat erhalten bleiben.
Sie gehören NICHT zwingend in dasselbe ZIP, aber sie dürfen nicht verloren gehen.

## R1 – FINAL FREEZE / TokenCache – ERFORDERLICH
Aktueller zweiter Account: `TokenCache`
Historischer erster Account: `hbhghghg`

Auf dem aktuellen Screenshot sichtbar:
- `contrastive_encoders/`
- `embeddings/`
- `figures/`
- `tokens/`
- `FINAL_FREEZE_COMPLETE.json`
- weitere Freeze-CSVs/JSONs

Mindestens bewahren:
- `tokens/train_4k/`
- `tokens/calibration/`
- `tokens/iid_test/`
- `tokens/holdout_8k/`
- `contrastive_encoders/`
- `embeddings/`
- komplette übrige Freeze-Ausgabe

**Ja: die ~2,81-GB-Datei/Dataset sichern.**
Sie ist nicht nur „unnötiger Cache“, sondern der komplette Final-Freeze-Artefaktbestand.

## R2 – RoBERTa-base – ERFORDERLICH FÜR NEUBERECHNUNG
Aktueller zweiter Account: `RoBertaaaa/roberta-base`
Historisch: `ijhuioo/roberta-base`

**Ja: die ~1,79-GB-Datei/Dataset sichern.**
Für das reine Schreiben braucht man sie nicht, für eine vollständige Reproduktion schon.

## R3 – ENDGAME – ERFORDERLICH
Aktueller zweiter Account `Datasett` enthält:
- `dapt40k_bundle.pkl`
- `split_roles_and_holdout_cache_v2_ram_safe.pkl`

Zusätzlich auf dem alten Account den **vollständigen ursprünglichen ENDGAME-Bestand sichern**, falls
dort noch die DAPT40k-Encoder Seeds 42/52/62/72/82 unter `Phase3_results/.../dapt_encoders/40k/...`
liegen. `artifact_audit.json` des FINAL FREEZE verweist genau darauf.

Die zwei PKLs reichen für die neue Replikation, aber **nicht zwingend für eine vollständige
bitgenaue Wiederherstellung des ursprünglichen FINAL FREEZE ohne erneutes DAPT-Training**.

## R4 – FINAL-N10 FULL OUTPUT – NOCH ZU SICHERN
Der aktuelle lokale Bestand enthält die wichtigsten N10-CSVs und den Completion-Marker,
aber `FINAL_N10_COMPLETE.json` bestätigt zusätzlich:
- 8 Thesis-Tabellen,
- 19 PNG-Figuren,
- 5 neue DAPT-Encoder,
- 5 neue Contrastive-Encoder,
- Score-Caches / weitere Audits.

Der Finish-only-Lauf referenziert diesen vollständigen Kaggle-Output als Dataset `activelearning`.

**Diesen kompletten N10-Output unbedingt separat vom alten Account sichern.**
Das ist derzeit die größte Lücke im lokalen BA-Archiv.

## R5 – PRODUKTIVER LOOP FULL STATECACHE `lpppll` – ERFORDERLICH
Komplett sichern:
- `LOOP_selection_history.json`
- `state_scores/*.npz`
- sämtliche LOOP-CSVs/Audits

Das kleine BA-Paket enthält die finalen CSVs, aber nicht die vielen State-Score-Dateien.
`lpppll` hat uns bereits Stunden Rechenzeit erspart.

## R6 – ORIGINAL10 AL×SSL FULL STATECACHE – EMPFOHLEN
Das Analysis-ZIP enthält alle finalen Tabellen/Statistiken, aber nicht die großen T0-State-NPZs.
Wenn der vollständige Kaggle-Output des E06-Laufs noch existiert, ebenfalls sichern.
Nicht zwingend für die BA-Auswertung, aber wertvoll für Neuauswertungen ohne Retraining.

## R7 – INDEPENDENT REPLICATION10
Nach Abschluss:
- mindestens Analysis-ZIP + Completion/Audits sichern,
- wenn ein kompletter Kaggle-Output mit Score-States existiert: ebenfalls archivieren.

## Empfohlene physische Struktur
```
Bachelor_Archiv/
├── BA_MASTER_V2_AUDITED/       # klein; Schreiben/Evidenz
└── REPRO_ASSETS/               # groß; Reproduzierbarkeit
    ├── R1_TokenCache/
    ├── R2_RoBERTaBase/
    ├── R3_ENDGAME_FULL/
    ├── R4_FINAL_N10_FULL/
    ├── R5_lpppll_FULL/
    ├── R6_AL_SSL_STATECACHE/
    └── R7_REPLICATION10_FULL/
```
