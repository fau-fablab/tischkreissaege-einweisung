Tischkreissäge Einweisung
=========================

Einweisung des [FAU FabLab](https://fablab.fau.de) für die Feinschnitt-Tischkreissäge [Proxxon FET](https://www.proxxon.com/de/micromot/27070.php).

Dies ist ein inoffizielles Dokument des FAU FabLab und steht in keiner Verbindung zu Proxxon.
„Proxxon“ ist eine Marke ihres Inhabers und wird hier nur zur Bezeichnung des Produkts verwendet.

Inhalt
------

- Regeln und Sicherheit, Betriebsanweisung (Aushang an der Säge, standardmäßig aus)
- Technische Daten, die wichtigsten Teile (eigene Skizze), bestimmungsgemäße Verwendung
- Vorbereitung: Checkliste, Schutzausrüstung, Aufstellen und Absaugung, Material, Sägeblatt wählen
- Einstellungen: Schnitthöhe, Neigung, Längsanschlag, ausziehbarer Tisch mit Hilfsanschlag, Winkelanschlag
- Sägen: Längs- und Querschnitt, Rückschlag, kleine Teile und Leiterplatten, Verbote
- Nach dem Sägen, Infos für Betreuer: Sägeblattwechsel, typische Fehler, Pflege

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/tischkreissaege-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/tischkreissaege-einweisung/Einweisung_Tischkreissaege.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/tischkreissaege-einweisung/Einweisungsliste_Tischkreissaege.pdf)

Die Betriebsanweisung (`betriebsanweisung/ba_tischkreissaege.tex`, BA-TK-01) ist noch ein Entwurf und wird
standardmäßig nicht gebaut. Zum Einschalten im `Makefile` die Zeile `TARGET += Betriebsanweisung_Tischkreissaege`
einkommentieren, dann erscheint sie als eigenes PDF und als Seite in der Einweisung
(siehe [README_betriebsanweisung.md](https://github.com/fau-fablab/fablab-document/blob/master/README_betriebsanweisung.md)).

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/tischkreissaege-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/tischkreissaege-einweisung.git
cd tischkreissaege-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/tischkreissaege-einweisung/status.svg)](https://brain.fablab.fau.de/build/tischkreissaege-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/tischkreissaege-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/tischkreissaege-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/tischkreissaege-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/tischkreissaege-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)

Die Einweisung und die Betriebsanweisung sind selbst formuliert und enthalten keine Texte oder Abbildungen aus der
Proxxon-Betriebsanleitung. Alle Zeichnungen in `zeichnungen/` sind selbst erstellte TikZ-Skizzen, die Sicherheitszeichen
(ISO 7010, gemeinfrei bzw. CC0) kommen aus fablab-document.
**Beim Bearbeiten nichts aus der Proxxon-Anleitung übernehmen, auch nicht sinngemäß Satz für Satz.** Bilder bitte
selbst fotografieren oder nur mit freier, kompatibler Lizenz (z. B. CC BY-SA von Wikimedia Commons, mit Quellenangabe)
verwenden.
