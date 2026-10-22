# Serge Paperface → Eurorack

Modulfamilie: die Serge-Paperface-Module (73-75-Schaltungen) als Eurorack-Module.
Jedes Modul bekommt einen eigenen Ordner unter `modules/` mit Hardware-Revisionen, Panel und Dokumentation.
Gemeinsame Vorgaben stehen in [`docs/konventionen.md`](docs/konventionen.md).

## Module

| Modul | Ordner | Stand | Fertigungsfreigabe |
|---|---|---|---|
| Envelope | [`modules/envelope`](modules/envelope) | REV1: KiCad-Projekt komplett geroutet, ERC/DRC 0 Meldungen | nein – mechanische Prüfung und Prototyp offen |
| VCO (Oszillator) | [`modules/vco`](modules/vco) | REV1: KiCad-Schaltplan vollständig, Platine platziert, noch unverdrahtet, ERC/DRC offen | nein |
| Triple Waveshaper, Peak/Trough, Comparator, Dual Processor, Gate, Ring, Reverb, Preamp, Positive/Negative Slew | `modules/<modul>` | Originalauszüge abgelegt, noch kein KiCad | nein |

Neue Module: [`modules/_vorlage`](modules/_vorlage) kopieren und umbenennen. Bauteilwahl: [`docs/bauteilregel.md`](docs/bauteilregel.md). Gemeinsame KiCad-Bibliotheken: [`shared/kicad`](shared/kicad).

## Weitere Inhalte

- [`system/panel-layout`](system/panel-layout) – Gesamt-Panel-Layout (Vectorworks + PDF-Export).

## Lizenz

Noch nicht festgelegt. Die Schaltungen beruhen auf den Serge-73-75-Build-Unterlagen; deren Rechte liegen bei den
jeweiligen Urhebern. Auszüge aus den Originalunterlagen nicht ohne Klärung öffentlich stellen.
Fremdbibliotheken behalten ihre Lizenz (z. B. `LICENSE_AudioJacks.txt`, MIT, im Envelope-Projekt).
