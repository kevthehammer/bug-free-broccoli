# Testbatterie

**Zweck dieser Datei:** Sie legt fest, wann und wie die Leistungstests durchgeführt werden, und ordnet die Ergebnisse ein. Die Tests dienen der Steuerung des Programms und dem Vergleich der Testzeitpunkte.

## Testzeitpunkte

- Woche 0, Woche 8 (nach Block 2), Woche 16 (nach Taper).
- Gleiche Tageszeit, gleiches Schuhwerk, gleiche Aufwärmroutine.
- Mindestens 48 h nach einer harten Einheit.

## Testablauf

Reihenfolge einhalten:

0. Basisdaten
1. Gesundheits-/Schmerz-Scores
2. Beweglichkeit
3. Sprünge
4. Agilität
5. Maximalkraft

Begründung: Ermüdungssensible Tests kommen zuerst, damit Ermüdung aus den späteren Tests die Ergebnisse nicht verfälscht.

## Tests

| Gruppe | Test | Durchführung | Messgröße | Richtwert |
| --- | --- | --- | --- | --- |
| Basisdaten | Körpergewicht | morgens nüchtern | kg | Referenz für relative Kraftwerte |
| Basisdaten | Standing Reach | Reichhöhe einarmig im Stand | cm | Basiswert für alle Sprungtests |
| Schmerz-Scores | VISA-P | standardisierter Fragebogen Patellasehne | 0–100 Punkte | unter 80 = relevante Tendinopathie |
| Beweglichkeit | Knee-to-Wall | Sprunggelenk-Dorsalextension | cm L/R | mindestens 10 cm, Seitendifferenz unter 1,5 cm |
| Beweglichkeit | Schulter-ROM | schmerzfreie Flexion, Außen-/Innenrotation 90° abduziert | Grad L/R | Seitendifferenz dokumentieren |
| Sprünge | Block Jump Reach | beidbeinig aus dem Stand, beide Arme | cm über Standing Reach | 45–60 cm ambitioniert Amateur |
| Sprünge | Approach Jump Reach | 3-Schritt-Anlauf, Angriffssprung | cm über Standing Reach | 55–75 cm ambitioniert Amateur |
| Sprünge | CMJ ohne Arme | Counter Movement Jump, Hände an der Hüfte | cm | isoliert Beinleistung ohne Armschwung |
| Sprünge | Single-leg CMJ L/R | je 3 Versuche pro Bein, bester Wert | cm + Asymmetrie in % | Asymmetrie unter 10 % |
| Agilität | 5-10-5 Pro-Agility | Standardaufbau 2× 4,57 m | s | beide Startrichtungen testen |
| Maximalkraft | 3RM Back Squat | nach vollem Aufwärmen | kg → 1RM via Epley | relative Kraft mindestens 1,5× Körpergewicht anstreben |
| Maximalkraft | 3RM Trap Bar Deadlift | high handles | kg → 1RM | — |
| Maximalkraft | 3RM Bench Press | nur bei schmerzfreier Schulter, sonst auslassen | kg → 1RM | — |
| Maximalkraft | Max Chin-ups | strikt, volle ROM | Wdh | Zielkorridor 10–15 |

## Die drei Reichhöhen messen

Die Reichhöhe ist, wie hoch der ausgestreckte Arm kommt, nicht wie hoch gesprungen wird. Im
Volleyball ist sie die wichtigere Zahl, weil am Netz die absolute Höhe zählt. Die Sprunghöhe ist
die Differenz aus Sprung- und Standreichhöhe.

| Wert | Ausführung |
| --- | --- |
| Standreichhöhe | Flach an der Wand stehen, Füße am Boden, Schlagarm maximal hoch, Schulter mitschieben. Fingerspitze markieren |
| Blockreichhöhe | Aus dem Stand beidbeinig hoch, beide Arme |
| Angriffsreichhöhe | Mit 3-Schritt-Anlauf, ein Arm, der Schlagarm |

Durchführung: Kreide oder Magnesia an die Fingerspitzen, an einer Hallenwand erst im Stand
antippen, dann springen und antippen, danach mit dem Maßband vom Boden zur Markierung messen.
Aufgewärmt, aber nicht ermüdet, drei Versuche je Wert, der beste zählt.

Bezugspunkt: Die Netzhöhe im Herrenbereich beträgt 2,43 m. Die Angriffsreichhöhe minus 2,43 m
ergibt, wie weit über Netzkante geschlagen wird. Diese Zahl sagt über die Wirkung im Spiel mehr
aus als jeder Kraftwert.

## Asymmetrie berechnen

`Asymmetrie % = (stärkeres Bein − schwächeres Bein) / stärkeres Bein × 100`

Rechenbeispiel: 42 cm und 38 cm ergeben (42 − 38) / 42 × 100 = 9,5 %.

Der Zielwert liegt unter 10 %. Bezugsgröße ist immer das stärkere Bein, damit die Werte über die drei Testzeitpunkte vergleichbar bleiben.

## Epley-Formel

Die 1RM-Schätzung aus einem Submaximalsatz:

`1RM = Gewicht × (1 + Wiederholungen / 30)`

Rechenbeispiel: 100 kg × 3 Wdh → 100 × (1 + 3 / 30) = 110 kg.

## Interpretation

Fortschrittsmarken nach 16 Wochen für fortgeschrittene Athleten:

- CMJ +3–6 cm
- Approach Jump +4–8 cm
- Squat-1RM +8–15 %
- Asymmetrie-Reduktion
- VISA-P +10–20 Punkte

Sprungzuwächse verlaufen nicht linear. Sie werden im Block 4 am sichtbarsten.

## Verweise

- [README.md](../README.md)
- [docs/01-athletenprofil.md](01-athletenprofil.md)
- [docs/03-periodisierung.md](03-periodisierung.md)
- [docs/11-prehab-knie.md](11-prehab-knie.md)
- [docs/12-prehab-schulter.md](12-prehab-schulter.md)
- [docs/15-progression-autoregulation.md](15-progression-autoregulation.md)
- [log/testprotokoll-vorlage.md](../log/testprotokoll-vorlage.md)
