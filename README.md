# Simulationen für den Physikunterricht

Browserbasierte Simulationen für den Physikunterricht. Jede Simulation ist **eine einzige HTML-Datei**:
herunterladen (z. B. aus Teams oder Moodle) und per Doppelklick im Browser öffnen. Es ist keine Installation
und keine Internetverbindung nötig.

## Startseite

`index.html` ist die Startseite (Tafel & Heft mit einem Sonnensystem der Themengebiete). Mit GitHub Pages ist sie unter
`https://crakestone.github.io/physicssimulations/` erreichbar.

**Neue Simulation eintragen:** In `index.html` in der Liste `SIMS` einen Eintrag ergänzen (Themengebiet, Titel,
Dateipfad, Kurztext, Schlagwörter). Ein neues Themengebiet kommt in die Liste `TOPICS` und erscheint automatisch als
neuer Planet. Jede Simulation ist ein Mond ihres Themen-Planeten.

## Übersicht

| Ordner | Simulation | Inhalt |
|---|---|---|
| `Stoßprozesse/` | `Stoss-Simulation.html` | Elastischer, plastischer (und teilelastischer) Stoß zweier Autos, gerade und schief |
| `Vektorfelder/` | `Feldlabor.html` | Elektrische, magnetische und Gravitationsfelder als strömende Teilchen, Feldlinien, Pfeile und Äquipotentiallinien; 51 Versuche, Baukasten, eigene Funktionen, 2D- und 3D-Ansicht |
| `Stromkreise/` | `Stromkreislabor.html` | Stromkreise bauen; Potenzial als Farbe, Höhe oder Elektronendruck; 12 Versuche, Messgeräte und Messspitzen |
| `Quantenphysik/` | `Quantenlabor.html` | Photoeffekt, Spektren, Doppelspalt mit Einzelobjekten (mit Zeigermodell) und Mach-Zehnder-Interferometer mit Quantenradierer |

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

## Vektorfelder – Feldlabor.html

- Darstellung wie bei *Fieldplay*: Tausende Teilchen strömen mit dem Feld. Dazu lassen sich **Feldlinien**,
  **Pfeile**, **Äquipotentiallinien** und **Achsen** zuschalten.
- **51 fertige Versuche** mit Vorschaubild, Erklärung und Frage für den Unterricht: Elektrisch, Magnetisch,
  Gravitation und Mathe & Strömung (Phasenraum, Räuber-Beute, Zylinderumströmung …), dazu Versuche speziell für 3D (Dipol im Raum, Potentialgebirge, Gravitationstrichter, Elektron in der Spule).
  Antippen lädt einen Versuch. Zieht man die Kachel ins Feld, wird er zum bestehenden Feld **hinzugefügt** (Superposition).
- **Baukasten:** Ladungen, Stab- und Hufeisenmagnet, Stromleiter, Spule, Kondensator, Metallkugel, Planeten,
  Hohlkugel, Kompass und Messsonde per Drag & Drop. Ein angetipptes Objekt zeigt Regler für Stärke, Größe und Drehung.
- **Probekörper** (Testladung, Elektron, Satellit) bewegen sich im Feld und zeichnen ihre Bahn.
  Die Startgeschwindigkeit stellt man über die Pfeilspitze ein.
- **Eigene Funktion** in Schulschreibweise: `Fx = -y`, `Fy = x` oder ein Potential `φ = x^2 + y^2`.
  Dazu kommen homogene Zusatzfelder (E, g, B senkrecht zur Ebene) und ein mitrotierendes Bezugssystem (Lagrange-Punkte).
- **Spule, Leiterschleife und Helmholtz-Spulenpaar** werden räumlich nach Biot-Savart berechnet.
  In 2D sieht man den Schnitt durch die Achse, in 3D die Windungen bzw. den Ring
  und z. B. die Schraubenbahn eines Elektrons in der Spule.
- **2D / 3D umschaltbar** (oben rechts):
  - *Raumfeld:* Ladungen, Magnete und Planeten liegen im Raum; Feldlinien und Teilchen laufen in alle Richtungen.
    Objekte lassen sich auch in die Höhe verschieben (Regler „Höhe z“ oder Alt + Ziehen).
    Die 2D-Ansicht ist der Schnitt durch die Grundebene z = 0.
  - *Landschaft:* das Potential als Gebirge bzw. Gummituch (Gravitationstrichter, Potentialberge und -täler,
    Lagrange-Punkte); Teilchen und Probekörper laufen darauf bergab.
  - Kamera: Ziehen dreht, Shift oder rechte Maustaste verschiebt, Mausrad bzw. zwei Finger zoomen;
    „Drehen“ lässt die Szene langsam kreisen. Eigene Funktionen können in 3D zusätzlich `Fz(x, y, z)` haben.
- Heller Hintergrund für den Beamer, Vollbild. Tasten: Leertaste = Pause, Entf = Objekt löschen.

Modell: relative Einheiten (k = G = 1). Magnete werden als zwei Pole berechnet. Kondensatorplatten und
gerade Stromleiter werden im Querschnitt gerechnet (senkrecht zur Bildebene unendlich lang, im 3D-Raumfeld daher als lange senkrechte Leiter bzw. Platten dargestellt).

## Stromkreise – Stromkreislabor.html

Ziel: Die Spannung als **Potenzialdifferenz** sichtbar machen – die häufigste Fehlvorstellung ist, dass Spannung eine
Eigenschaft des Stroms sei.

- **Baukasten auf einem Steckbrett:** Kabel (von Punkt zu Punkt zeichnen), Batterie, Lämpchen, Widerstand, Schalter,
  Strom- und Spannungsmessgerät aus der Leiste aufs Brett ziehen. Antippen öffnet die Einstellungen (Spannung, Widerstand,
  Umdrehen, Entfernen); zurück auf die Leiste ziehen löscht. Rückgängig mit Strg+Z.
- **Drei Ansichten:**
  - *Farbe:* Jedes Kabel hat die Farbe seines Potenzials (blau = Minuspol, rot = Pluspol). Eine Spannung ist ein
    Farbunterschied. Über einem Kabel zeigt die Maus das Potenzial an.
  - *Höhe:* Höhenmodell in Schrägansicht – die Batterie hebt die Ladungen an, im Lämpchen rollen sie hinunter.
  - *Elektronengas:* Frankfurter Elektronengasmodell – viele Elektronen (hoher Druck) am Minuspol, wenige am Pluspol;
    Lämpchen und Widerstände als Engstellen.
- **Messspitzen:** zwei frei bewegliche Spitzen messen die Spannung zwischen beliebigen Punkten (z. B. am offenen Schalter).
- **12 Versuche** mit Frage und Erklärung: einfacher Stromkreis, Batterie ohne Lämpchen, offener Schalter, Reihe, parallel,
  überbrücktes Lämpchen, Kurzschluss, gemischte Schaltung, Spannungsteiler, zwei Batterien, „Wird Strom verbraucht?“, leerer Baukasten.
- **Drei Niveaustufen:** *Einfach* ohne Zahlenwerte an Bauteilen; *Mittel* mit U und I an den Bauteilen und U = R·I;
  *Anspruchsvoll* zusätzlich Leistung, Knotenregel (Maus auf einen Knoten) und Innenwiderstand der Batterie.
- Lämpchen brennen bei zu hoher Leistung durch, ein Kurzschluss wird gemeldet.

Modell: Knotenpotenzialverfahren; Kabel 0,0001 Ω, Lämpchen als ohmsche Widerstände (Helligkeit ∝ Leistung),
Batterie mit sehr kleinem Innenwiderstand und Strombegrenzung bei Kurzschluss (20 A). Bezugspunkt φ = 0 ist der Minuspol.

## Quantenphysik – Quantenlabor.html

Vier Stationen (oben umschaltbar, auch direkt über `#photoeffekt`, `#spektren`, `#doppelspalt`, `#interferometer`),
jeweils mit Aufträgen und Erklärungen:

- **Photoeffekt:** Lampe mit einstellbarer Wellenlänge (200–800 nm) und Helligkeit, sechs Metalle, Photonen und
  herausgelöste Elektronen, Energiediagramm (Photonenenergie, Austrittsarbeit, Bewegungsenergie). Ab *Mittel*:
  Gegenspannung. *Anspruchsvoll:* Messpunkte speichern, Ausgleichsgerade, Bestimmung von h, Grenzfrequenz und W.
- **Spektren:** Leuchtröhren (H, He, Na, Hg, Ne) und Absorption (weißes Licht durch Gas). Beim Wasserstoff ein
  Energieniveauschema zum Antippen: Das Elektron fällt zurück und sendet Photonen aus (Lyman im UV, Balmer sichtbar,
  Paschen im IR). Rätselgas mit Vergleichsspektren.
- **Doppelspalt:** Photonen (400–700 nm) oder Elektronen (2–50 kV, λ = h/p) einzeln oder in großer Zahl; Schirm mit
  Einschlägen, Histogramm und Wahrscheinlichkeitskurve; einen Spalt schließen; Welcher-Weg-Detektor. Ab *Mittel*:
  Zeigermodell für einen antippbaren Punkt am Schirm.
- **Interferometer (Mach-Zehnder):** einzelne Photonen oder Laserlicht, Glasplatte als Phasenschieber, Wege blockieren,
  zweiten Strahlteiler entfernen, Zähler mit berechneter Wahrscheinlichkeit, Zeiger an den Detektoren. *Anspruchsvoll:*
  Polarisationsfilter (Weginformation) und 45°-Filter als Quantenradierer.

Modell: Austrittsarbeiten Cs 2,14 · K 2,29 · Na 2,36 · Zn 4,33 · Cu 4,65 · Pt 5,65 eV; Doppelspalt mit
I ∝ cos²(π d sinθ/λ)·sinc²(π b sinθ/λ) und Abstand 1 m; Interferometer mit Strahlteiler-Amplituden 1/√2 und i/√2,
Photonen unter 45° polarisiert. Die Stromstärke am Photoeffekt ist schematisch (ein Elektron je absorbiertem Photon).

## Navigation

In jeder Simulation führt ein Klick auf den Titel oben links (z. B. „Feldlabor“, „Stromkreislabor“ oder „Quantenlabor“) zurück zur Startseite `index.html`.
