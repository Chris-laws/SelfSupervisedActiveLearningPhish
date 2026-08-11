# AL × SSL Interaction N10

Diese Analyse ist explorative/supportende Evidenz zur nachgelagerten
Active-Learning-Erweiterung. Sie ist keine Forschungsfrage und Active Learning
ist nicht Self-Supervised Learning.

## Primärer Test
Difference-in-Differences:
(DAPT_Uncertainty - DAPT_Random) - (T0_Uncertainty - T0_Random)

## Automatische Einordnung
DESCRIPTIVE_ONLY: Die Interaktion ist im Stressmittel positiv, aber statistisch nicht hinreichend abgesichert. Active Learning darf nicht als nachgewiesener SSL-Verstärker formuliert werden.

## Methodische Grenze
Der Interaktionstest vergleicht die operationalen Lernstrategien.
Da T0 und DAPT unter Uncertainty Sampling modellabhängig unterschiedliche
Fälle auswählen können, darf eine positive Interaktion nicht ohne zusätzliche
Analyse als kausaler Nachweis besserer DAPT-Unsicherheitskalibrierung
interpretiert werden.

## Reuse
- DAPT-AL-Ergebnisse: vorhandener produktiver Loop
- T0: neu gerechnet
- Random-Labelsets: T0 und DAPT exakt identisch
- 10%-Start: über alle Bedingungen identisch
