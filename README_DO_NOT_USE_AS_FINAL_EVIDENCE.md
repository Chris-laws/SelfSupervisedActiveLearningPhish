# LEGACY / ERSTES EXPERIMENT – NICHT ALS FINALE EVIDENZ VERWENDEN

Wichtig für die Trennung alter und finaler Versuchslinien:

## Historischer B0
Die 36 URL-/HTML-Strukturmerkmale stammen als **Merkmalsdefinition/gespeicherte Featurewerte**
aus der früheren B0-Versuchslinie. Diese Provenienz darf für die technische Herleitung genutzt werden.

**Nicht übernommen werden dürfen:**
- alte B0-Performancewerte,
- alter Split,
- alter Threshold,
- alte 5-/6k-Testzahlen,
- alte Modellrangfolgen.

Im FINAL-N10 wird `B0_STRUCT_XGB` auf den finalen 40k-aware Splits und Labelbudgets neu trainiert
und neu kalibriert. Nur diese N10-Zahlen sind finale Evidenz.

## Frühere Freeze-/Hybrid-Versionen
v1/v2/v3/v4 bzw. 5-Seed-Zwischenstände werden nur zur Historie behalten.
Wenn ein Befund in FINAL-N10 neu berechnet wurde, gilt ausschließlich FINAL-N10.

## Regel
Keine Zahl aus einem Legacy-/Pilot-/Superseded-Output in Kapitel Evaluation oder Diskussion
verwenden, sofern dieselbe Größe später unter dem finalen Protokoll neu berechnet wurde.
