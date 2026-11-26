# Simulationen für den Physikunterricht

Browserbasierte Simulationen für den Physikunterricht. Jede Simulation ist **eine einzige HTML-Datei**:
herunterladen (z. B. aus Teams oder Moodle) und per Doppelklick im Browser öffnen. Es ist keine Installation
und keine Internetverbindung nötig.

## Übersicht

| Ordner | Simulation | Inhalt |
|---|---|---|
| `Stoßprozesse/` | `Stoss-Simulation.html` | Elastischer, plastischer (und teilelastischer) Stoß zweier Autos, gerade und schief |

## Stoßprozesse – Stoss-Simulation.html

- Zwei Autos mit einstellbarer Masse und Geschwindigkeit, wählbar als **Modellautos (Labor)**
  (0,1–5 kg, m/s) oder **echte Fahrzeuge** (500–40 000 kg, km/h; vom Kleinwagen bis zum LKW).
- **Gerader Stoß** (Ansicht von der Seite und von oben) oder **schiefer Stoß** mit einstellbarem
  Stoßwinkel (z. B. Kreuzungsunfall unter 90°).
- **Stoßart als Spektrum:** Schieberegler „Umgewandelte Energie“ von 0 % (elastisch) bis 100 % (plastisch);
  dazwischen teilelastisch. Auf „Anspruchsvoll“ wird zusätzlich die Stoßzahl k = √(1 − Anteil) angezeigt.
- **Drei Niveaustufen** für die Anzeige:
  - *Einfach:* Geschwindigkeit und Impuls mit Richtungspfeilen, Gesamtimpuls, einfacher Rechenweg.
  - *Mittel:* zusätzlich Bewegungsenergie, Energieverlust und die Stoßformeln mit eingesetzten Zahlen.
  - *Anspruchsvoll:* Komponenten, Schwerpunktgeschwindigkeit, Stoßzahl, reduzierte Masse,
    Schwerpunkt-Anzeige und Schwerpunktsystem.
- **Zeit-Diagramme:** v‑t, p‑t, E‑t und x‑t, die mit der Animation mitlaufen.
- Impulsdiagramm (Pfeiladdition), Energiebalken, automatische Beobachtungen.
- **Großansicht** für den Beamer: nur die Animation (auf Wunsch mit Diagramm) im Vollbild,
  mit einer Zeile mit den wichtigsten Werten. Taste G.
- **Übungsmodus:** Die Ergebnisse bleiben verborgen, bis man sie aufdeckt.
- Zeitlupe, Zeitregler, „beim Stoß anhalten“, Vollbild für den Beamer.
  Tasten: Leertaste = Start/Pause, R = zurück, G = Großansicht.

Modell: Die Fahrzeuge werden wie Massepunkte behandelt (zentraler Stoß, keine Reibung, keine Drehung).
Gerechnet wird exakt mit Impulserhaltung und der Stoßzahl k: v' = (1 + k)·v_S − k·v.
