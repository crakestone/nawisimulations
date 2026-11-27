# Simulationen für den Physikunterricht

Browserbasierte Simulationen für den Physikunterricht. Jede Simulation ist **eine einzige HTML-Datei**:
herunterladen (z. B. aus Teams oder Moodle) und per Doppelklick im Browser öffnen. Es ist keine Installation
und keine Internetverbindung nötig.

## Startseite

`index.html` ist die Startseite „NaWi zum Ausprobieren“ (Tafel & Heft mit einem Sonnensystem der Fächer). Mit GitHub Pages
ist sie unter `https://crakestone.github.io/physicssimulations/` erreichbar.

Jedes **Fach** ist ein Planet (Physik, Chemie, Biologie, Mathematik, Informatik, Geographie), jede Simulation ein Mond
ihres Fach-Planeten. Fächer ohne Simulation werden als „noch leer“ angezeigt. Ein Klick auf einen Planeten zeigt darunter
nur die Simulationen dieses Fachs.

**Neue Simulation eintragen:** In `index.html` in der Liste `SIMS` einen Eintrag ergänzen: Fach (`subject`, Pflicht),
Themengebiet innerhalb des Fachs (`topic`, optional, erscheint als Etikett auf der Karte), Titel, Dateipfad, Kurztext,
Schlagwörter. Ist nicht klar, in welches Fach eine neue Simulation gehört: nachfragen. Ein neues Fach kommt in die Liste
`SUBJECTS` und erscheint automatisch als neuer Planet; neue Themengebiete kommen in `TOPICS`.

## Übersicht

| Ordner | Simulation | Inhalt |
|---|---|---|
| `Stoßprozesse/` | `Stoss-Simulation.html` | Elastischer, plastischer (und teilelastischer) Stoß zweier Autos, gerade und schief |
| `Vektorfelder/` | `Feldlabor.html` | Elektrische, magnetische und Gravitationsfelder als strömende Teilchen, Feldlinien, Pfeile und Äquipotentiallinien; 51 Versuche, Baukasten, eigene Funktionen, 2D- und 3D-Ansicht |
| `Stromkreise/` | `Stromkreislabor.html` | Stromkreise bauen; Potenzial als Farbe, Höhe oder Elektronendruck; 12 Versuche, Messgeräte und Messspitzen |
| `Bandstruktur/` | `Bandstrukturlabor.html` | Freies Elektron, reziproker Raum und Brillouin-Zonen, Kronig-Penney, Bragg-Reflexion, Tight-Binding, Bänder füllen, Si und GaAs |
| `Halbleiter/` | `Halbleiterlabor.html` | Bändermodell, Dotierung, innerer und äußerer Photoeffekt, pn-Übergang, Solarzelle, LED |
| `Quantenphysik/` | `Quantenlabor.html` | Photoeffekt, Spektren, Doppelspalt mit Einzelobjekten (mit Zeigermodell) und Mach-Zehnder-Interferometer mit Quantenradierer |
| `Relativitätstheorie/` | `Relativitaetslabor.html` | Lichtuhr und Myonen, Gleichzeitigkeit, Längenkontraktion (Leiter-Garage), Geschwindigkeitsaddition, Zwillingsparadoxon, Raumzeit-Diagramm, Lichtmauer & E = mc², GPS, Doppler-Effekt; Wechsel des Bezugssystems |

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

## Relativitätstheorie – Relativitaetslabor.html

Neun Stationen (auch direkt über `#lichtuhr`, `#gleichzeitigkeit`, `#laengenkontraktion`, `#geschwindigkeiten`, `#zwillinge`,
`#raumzeit`, `#lichtmauer`, `#gps`, `#doppler`), jeweils mit Aufträgen, Erklärungen und drei Niveaustufen.

- **Sicht wechseln:** Über der Szene schaltet „Sicht von: Bahnsteig | Zug“ (bzw. Erde | Rakete, Garage | Leiter …) das
  Bezugssystem um. Die Szene geht dabei fließend in die andere Sicht über (Lorentz-Transformation). Taste B wechselt die Sicht.
- **Welt:** „Echte Welt“ oder Gedankenwelt mit c = 20 km/h (wie bei Mr Tompkins): Geschwindigkeiten und Zeiten werden in
  Alltagsgrößen angezeigt.
- **Lichtuhr:** zwei Lichtuhren (Bahnsteig, Zug) mit Lichtspur im Zickzack und Tick-Zählern; ab *Mittel* γ und Dreieck nach
  Pythagoras, *Anspruchsvoll* mit Herleitung. Szene **Myonen**: Schauer aus 500 Myonen in 15 km Höhe, Zerfall nach der
  Eigenzeit, Vergleich mit klassischer Rechnung; in der Sicht der Myonen ist die Atmosphäre verkürzt.
- **Gleichzeitigkeit:** Einsteins Zug mit zwei Blitzen, Lichtkreisen, Brandflecken und Lämpchen bei Paula (Bahnsteig) und
  Toni (Zug); Blitze gleichzeitig für Bahnsteig oder Zug; ab *Mittel* synchronisierte Uhren und Minkowski-Diagramm.
- **Längenkontraktion:** Zug und Tunnel gleicher Ruhelänge mit Maßstäben; *Anspruchsvoll:* Leiter-Garage-Paradoxon mit Toren.
- **Geschwindigkeiten:** Rakete schießt Kugel oder Lichtblitz; Alltagsregel und Einstein nebeneinander, Diagramm u(v),
  *Anspruchsvoll:* Stufenrakete und Rapidität.
- **Zwillinge:** Reise mit einstellbarer Geschwindigkeit und Entfernung, Geburtstagsgrüße als Lichtsignale, Alter beider
  Zwillinge, Sicht der Hin- und Rückflug-Rakete; Minkowski-Diagramm mit Gleichzeitigkeitslinien und „Sprung“ beim Umkehren.
- **Raumzeit:** Ereignisse ins Minkowski-Diagramm setzen und ziehen, System S′ mit einstellbarer Geschwindigkeit,
  Lichtkegel, Koordinaten in S und S′, zeitartig/raumartig/lichtartig, Gitter von S′, Eichhyperbeln, „Jetzt“-Linie.
- **Lichtmauer & E = mc²:** Elektron (Myon, Proton) mit 1 keV bis 10 TeV; Rennen gegen das Licht auf 8,4 m (wie bei
  Bertozzi 1964), Geschwindigkeit über der Energie klassisch und relativistisch, Energie und Impuls, E = mc² mit Haushalten.
- **GPS:** Satellitenuhr in einstellbarer Höhe (ISS, GPS, Galileo, geostationär); SRT und ART einzeln schaltbar,
  Positionsfehler im Navi, Gangunterschied über der Höhe; *Anspruchsvoll:* Verstimmung ab Werk.
- **Doppler-Effekt:** Rakete sendet Licht wählbarer Farbe, Wellenberge als Kreise, Farben bei den Personen vorne und hinten;
  Vergleich ohne Zeitdilatation; *Anspruchsvoll:* transversaler Doppler-Effekt.

Modell: Rechnung mit c = 1. Die Szenen sind als Weltlinien im Bahnsteig- bzw. Erdsystem beschrieben und werden für die
Anzeige exakt in das gewählte Bezugssystem transformiert. Myonen: mittlere Lebensdauer 2,197 µs. GPS: GM = 3,986·10¹⁴ m³/s²,
R = 6371 km, Kreisbahn, Erddrehung vernachlässigt (GPS: −7,2 µs + 45,7 µs = +38,5 µs pro Tag).
Doppler: λ = γ·λ₀·(1 − β·cos θ) mit dem Winkel beim Aussenden.

## Halbleiter – Halbleiterlabor.html

Sechs Stationen (auch direkt über `#baender`, `#dotierung`, `#photoeffekt`, `#diode`, `#solarzelle`, `#led`), jeweils mit
Aufträgen, Erklärungen und drei Niveaustufen:

- **Bänder:** Energieniveaus von 1, 2, … sehr vielen Atomen spalten bei kleinem Abstand zu Bändern auf (Tight-Binding-Schema).
  Kristall aus Kupfer, Germanium, Silizium, Galliumarsenid oder Diamant mit Valenz- und Leitungsband, Temperatur,
  angelegter Spannung und Licht (Fotoleitung). Spezifischer Widerstand über der Temperatur (logarithmisch).
- **Dotierung:** Siliziumgitter mit Bindungselektronen neben dem Bändermodell; Phosphor (Donator, fünftes Elektron) und
  Bor (Akzeptor, Lochwanderung durch springende Elektronen), Eigenleitung bei hoher Temperatur, Drift im Feld, Fermi-Niveau.
- **Photoeffekt außen & innen:** dasselbe Licht (200–2000 nm) auf ein Metall und einen Halbleiter im selben Energiemaßstab;
  Austrittsarbeit gegen Bandlücke, Thermalisierung, Fotowiderstand (z. B. CdS).
- **Diode:** p- und n-Gebiet mit Löchern, Elektronen und ortsfesten Ionen; Raumladungszone, die mit der Spannung schmaler
  oder breiter wird; Bandverbiegung mit Fermi-Niveaus; Stromkreis mit Lämpchen; Kennlinie nach Shockley (Si und Ge).
- **Solarzelle:** Querschnitt mit logarithmischer Tiefe, Photonen aus dem Sonnenspektrum oder einfarbig, Eindringtiefe je
  nach Wellenlänge, Trennung der Ladungsträger, Ventilator als Verbraucher; Kennlinie mit Leistungskurve, MPP und
  Widerstandsgerade; Verlustbilanz; Temperatur; Modul mit bis zu 60 Zellen; Wirkungsgrad je nach Bandlücke.
  Materialien: Si, CIGS, GaAs, CdTe, Perowskit, Ge.
- **LED:** Stromkreis mit Vorwiderstand (oder ohne – dann brennt sie durch), Rekombination im Bändermodell, Spektrum,
  sieben Farben und weiße LED; *Anspruchsvoll:* Bestimmung von h aus Schwellspannung und Frequenz.

Modell der Solarzelle: Sonnenspektrum als Schwarzer Strahler (5778 K) auf die Bestrahlungsstärke skaliert,
Quantenausbeute 90 %, Zellfläche 100 cm², Diodengleichung mit I₀ ∝ e^(−E_g/kT), so kalibriert, dass Silizium bei 25 °C
U_oc = 0,63 V hat (Si: η ≈ 19 %, Füllfaktor 0,83, −1,6 mV/K). Eigenleitungsdichte n_i = √(N_C·N_V)·(T/300 K)^1,5·e^(−E_g/2kT).
Die Zahl der gezeichneten thermischen Ladungsträger ist logarithmisch skaliert.

## Bandstruktur – Bandstrukturlabor.html

Sieben Stationen (auch direkt über `#freies-elektron`, `#reziproker-raum`, `#kristallpotential`, `#bragg`, `#atome-band`,
`#baender-fuellen`, `#si-gaas`), jeweils mit Aufträgen, Erklärungen und drei Niveaustufen:

- **Freies Elektron:** Parabel E = ħ²k²/(2m) mit den erlaubten Zuständen k = 2πn/(N·a) im Ring aus N Atomen; laufende Welle.
- **Reziproker Raum:** 2D-Gitter (quadratisch, rechteckig, hexagonal, schiefwinklig, frei einstellbar) neben dem reziproken
  Gitter; Gitterebenen zu einem angetippten Punkt G (d = 2π/|G|); Brillouin-Zonen 1–4 eingefärbt, Konstruktion über
  Mittelsenkrechten; Elektronenwelle k zum Ziehen mit Anzeige der Bragg-Bedingung |k| = |k − G|; Beugungsbild.
- **Kristallpotential:** Kronig-Penney-Modell exakt gelöst; Potential mit den erlaubten Energiebereichen; E(k) im erweiterten,
  reduzierten und periodischen Zonenschema; Vergleich mit dem freien Elektron; Zustandsdichte.
- **Bragg:** fast freie Elektronen an der Zonengrenze; Mischung aus hin- und rücklaufender Welle, stehende Wellen mit
  |ψ|² bei den Rümpfen (unteres Band) bzw. dazwischen (oberes Band); Lücke 2|U|; Gruppengeschwindigkeit.
- **Atome → Band:** Tight-Binding mit s- und p-Orbitalen, E(k) = E₀ − 2t·cos(ka), Bloch-Summe der Orbitale (bindend/antibindend),
  Niveauschema 1 Atom → N Atome, Bandbreite über den Atomabstand.
- **Bänder füllen:** 1–4 Elektronen pro Atom; besetzte Zustände, Fermi-Energie, Zustandsdichte; Metall/Halbleiter/Isolator;
  angelegte Spannung verschiebt die Besetzung (volles Band → kein Strom); Fermi-Dirac bei Temperatur.
- **Si & GaAs:** drehbare 1. Brillouin-Zone des fcc-Gitters (Oktaederstumpf) mit Γ, X, L, K; vereinfachte Bandstrukturen
  entlang L–Γ–X mit Energien nach Messwerten; Photonabsorption direkt (GaAs) bzw. mit Phonon (Si); effektive Masse.

Modell: ħ²/(2m_e) = 0,0381 eV·nm², Gitterkonstante der 1D-Modelle a = 0,4 nm.

## Navigation

In jeder Simulation führt ein Klick auf den Titel oben links (z. B. „Feldlabor“, „Stromkreislabor“, „Quantenlabor“, „Halbleiterlabor“, „Bandstrukturlabor“ oder „Relativitätslabor“) zurück zur Startseite `index.html`.
