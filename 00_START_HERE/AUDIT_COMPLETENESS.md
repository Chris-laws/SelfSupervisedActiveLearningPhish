# AUDIT – Ist der Bachelor-Ordner vollständig?

## Wissenschaftliche Governance
Die verbindliche Struktur folgt `../01_GOVERNANCE/Bachelorarbeit-THEMA.txt`:
genau FF1, FF2 und FF3; keine FF4. Kaskade und Active Learning sind
nachgelagerte prototypische bzw. explorative Erweiterungen des Software-Artefakts
und keine eigenständigen Forschungsfragen.

## Bestätigt lokal vorhanden
### Kanonische Notebooks
- E01 Core Freeze: `v5_resume`
- E02 Hybrid 5-Seed Support: `v3_resume`
- E03 FINAL N10: `N10_PRUEFSICHER`
- E04 Productive AL: ursprünglicher langer Loop (AL vollständig, Fehler erst beim optionalen SSL-Refresh)
- E05 SSL Refresh: `FINISH_ONLY_v2_FLAT_KAGGLE`
- E06 AL×SSL Original10: `FAST_3H30_v2_BUDGETKEY_FIX`
- E07 Independent Replication10: aktuelles laufendes Notebook

### Completion-Marker
- `FINAL_FREEZE_COMPLETE.json`: 675/675, COMPLETE
- `HYBRID_FREEZE_EXTENSION_COMPLETE.json`: COMPLETE (im Hybrid-ZIP)
- `FINAL_N10_COMPLETE.json`: 7560/7560 + 17280/17280 AL, COMPLETE
- `PRODUCTIVE_FINISH_ONLY_COMPLETE.json`: COMPLETE (im Finish-ZIP)
- `AL_SSL_INTERACTION_COMPLETE.json`: 50/50 T0 states, 720 rows, COMPLETE

## Historische/Fix-Notebooks
Sind vorhanden, aber ausschließlich unter `03_NOTEBOOK_HISTORY/`. Sie dürfen nicht mit finalen
Ergebnissen vermischt werden.

## Noch NICHT vollständig lokal
1. **vollständiger FINAL-N10-Kaggle-Output** (`activelearning`) mit allen 8 Tabellen, 19 Figuren,
   Replikationsencodern und Score-Caches.
2. **vollständiges `lpppll`** mit `state_scores` und `LOOP_selection_history.json`.
3. **große TokenCache-/RoBERTa-/ENDGAME-Artefakte** liegen außerhalb dieses Containers und müssen
   separat archiviert werden.
4. E07 Replication10 ist noch laufend.

## Konsequenz
Der aktuelle kleine Master ist vollständig genug für das **Schreiben mit den vorhandenen finalen
Ergebnisdateien**, aber erst nach Sicherung der externen R1–R7-Artefakte ist das Gesamtprojekt
vollständig reproduzierbar archiviert.
