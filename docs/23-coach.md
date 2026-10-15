# Die App als Coach

Stand 15.10.2026. Kev möchte, dass die App wie ein Coach arbeitet: Sie gibt den Tag vor, passt die
Einheit an Tagesform und Zeit an, erklärt Übungen, gibt nach dem Training Rückmeldung und passt die
Zielgewichte an. Die Zahlen kommen aus festen Regeln. Claude formuliert in der App nur die
Rückmeldung und beantwortet Fragen zu Übungen.

## Stufen

1. **Tages-Check, Zeit, Anpassung, Erklärungen, Bewertung, Zielgewichte, Feedback.** Umgesetzt in
   Version 18.
2. **Wochenplanung und Briefing.** Umgesetzt in Version 19. Unter „Woche planen“ lässt sich das
   Herrentraining als ausgefallen markieren und jede Krafteinheit verschieben oder streichen. Das
   Coach-Briefing steht oben auf „Heute“: letztes Feedback, Ziele heute, Woche, nächstes Spiel.
   Gespeichert unter `woche/<Montag>`.

## Verschieben (Praxisregeln)

Die App bietet nur Tage an, die diese Regeln erfüllen:

- nicht am Spieltag und nicht in der Vergangenheit
- keine zwei Krafteinheiten an einem Tag
- Kraft 1 und Kraft 3 mindestens zwei Tage vor dem Spiel, nicht am Tag nach dem Spiel und nicht direkt neben der anderen
- Kraft 2 mindestens einen Tag vor dem Spiel

Fällt in einer Woche ohne Spiel das Freitagstraining aus, schlägt die App vor, Kraft 3 auf Freitag
vorzuziehen.

## Wochenrahmen (fest)

Balltraining Dienstag und Freitag; Freitag fällt öfter aus. Spiele immer samstags laut Spielplan.

## Regeln

### Zeit

| Einheit | ca. 45 min | ca. 30 min |
| --- | --- | --- |
| Kraft 1 | ohne Pogo Hops und Waden; Sprint und RDL je ein Satz weniger | Kurzversion (Schlitten, Aufwärmen, Sprint, Squat, RDL) |
| Kraft 2 | ohne Copenhagen, Carry, Pallof, einarmiges Rudern; Serratus ein Satz weniger | Kurzversion |
| Kraft 3 | ohne Hanging Leg Raise | zusätzlich ohne Calf Raise und Lateral Bound, Anlaufsprung ein Satz weniger |

Wenig Zeit kostet wenig: Schon ein bis zwei schwere Sätze pro Übung erhalten und steigern Kraft
(Iversen 2021). Gestrichen wird von hinten nach Priorität, die Hauptübungen bleiben.

### Tagesform

Beine (frisch, normal, schwer) und Schlaf (gut, mittel, schlecht) ergeben 0 bis 4 Punkte.
Subjektive Angaben zeigen Belastung empfindlicher an als viele objektive Werte (Saw 2016).

- 3 bis 4 Punkte: Langhantelübungen ein Satz weniger, 5 % leichter. Praxisregel.
- 2 Punkte: Hinweis, den Satz bei langsamer Wiederholung zu beenden.

### Knie und Schulter

Die App übernimmt die Ampeln aus [11-prehab-knie.md](11-prehab-knie.md) und
[12-prehab-schulter.md](12-prehab-schulter.md).

- **Knie 4–5:** Sprünge halbiert, keine Kontrastsprünge, danach Spanish Squat.
- **Knie über 5:** Sprünge und Sprints fallen weg. Squat wird 10 % leichter und langsam.
- **Schulter mit Spannung:** kein Drücken.
- **Schulter 3–5:** zusätzlich Brustpass statt Überkopfwurf und Serratus ein Satz weniger.
- **Schulter über 5:** Würfe und Serratus fallen weg. Chin-ups bekommen einen Satz weniger und werden 10 % leichter. Abklären lassen.

### Zwicken (Praxisregeln)

- **Oberschenkel hinten:** ohne Sprint, Nordic und RDL.
- **Leiste:** ohne Copenhagen und Lateral Bound, Sprint ein Satz weniger.
- **Rücken:** ohne RDL, Squat und Clean 10 % leichter.
- **Wade oder Achilles:** ohne Sprünge, Sprint und explosive Waden.

Ein Zwicken heißt hier: die Struktur einen Tag lang nicht schnell oder exzentrisch belasten.
Dahinter steht keine Studie, das ist ein vorsichtiger Standard.

### Zielgewicht

Nach jeder Übung mit Gewicht bewertet Kev den letzten Satz nach Wiederholungen in Reserve
(RIR-Skala, Helms 2016):

| Bewertung | nächstes Mal |
| --- | --- |
| leicht, 4+ übrig | zwei Stufen mehr (Langhantel +5 kg, sonst +2 kg) |
| passend, 2–3 übrig, alle Sätze | eine Stufe mehr (+2,5 kg bzw. +1 kg) |
| schwer, 1 übrig | gleich |
| Grenze, 0 übrig | 5 % weniger |

Das folgt dem Prinzip der autoregulierten Steigerung (APRE, Mann 2010): Das Gewicht richtet sich
danach, was am Tag ging. Die Stufen selbst sind Praxiswerte. Wenn der Tagesplan ein Gewicht nennt
(etwa Squat-Rampe 80, 85, 90 kg), gilt der Plan. Nur nach „schwer“ oder „Grenze“ bleibt die App
darunter.

## Feedback

Nach dem Speichern bekommt Claude die Einheit: Plan, Gemachtes, Bewertungen, Check, Notiz und die
letzten zwei Einheiten derselben Art. Daraus schreibt Claude höchstens 110 Wörter: Plan eingehalten,
was gut lief, worauf achten. Claude ändert keine Zielgewichte. Das Feedback wird im Tagebuch
gespeichert (`log/<Datum>.coach`).

## Quellen

- Helms ER et al. (2016). Application of the repetitions in reserve-based rating of perceived exertion scale for resistance training. Strength Cond J 38(4).
- Mann JB et al. (2010). The effect of autoregulatory progressive resistance exercise vs. linear periodization on strength improvement in college athletes. J Strength Cond Res 24(7).
- Saw AE et al. (2016). Monitoring the athlete training response: subjective self-reported measures trump commonly used objective measures. Br J Sports Med 50(5).
- Iversen VM et al. (2021). No time to lift? Designing time-efficient training programs for strength and hypertrophy. Sports Med 51(10).
