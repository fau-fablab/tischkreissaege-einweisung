Tischkreissäge Einweisung
=========================

Einweisung des [FAU FabLab](https://fablab.fau.de) für die Feinschnitt-Tischkreissäge [Proxxon FET](https://www.proxxon.com/de/micromot/27070.php).

Inhalt
------

- Technische Daten, allgemeine Sicherheitshinweise, Schutzausrüstung
- Bestimmungsgemäße Verwendung, Inbetriebnahme, Sägeblattschutz
- Einstellungen: Höhe und Neigung des Sägeblatts, Sägetisch ausziehen, Sägeblatt wählen und wechseln
- Arbeiten mit Längs-, Hilfs- und Winkelanschlag

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/tischkreissaege-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/tischkreissaege-einweisung/Einweisung_Tischkreissaege.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/tischkreissaege-einweisung/Einweisungsliste_Tischkreissaege.pdf)

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

Ausnahme: Abbildungen, Tabellen und Textabschnitte aus der Proxxon-Betriebsanleitung; deren Rechte liegen bei Proxxon.
