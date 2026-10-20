# Konventionen für alle Module

## Ordnerstruktur pro Modul

```
modules/<modul>/
  README.md              Status, offene Punkte, Quellen
  hardware/revN/         KiCad-Projekt je Revision (Schaltplan, PCB, Gerber, Stückliste, ERC/DRC)
  panel/revN/            Frontplatte (DXF/PDF)
  docs/                  Quellen, Auszüge, Abgleich- und Messprotokolle
```

Alte Revisionen bleiben im Repo und werden im Modul-README als ersetzt/zurückgezogen markiert.

## Eurorack-Stromversorgung

10-Pin-Stecker (wie Envelope REV1): Pins 1/2 = −12 V (NC, wenn nicht benötigt), Pins 3–8 = Masse, Pins 9/10 = +12 V.
Rote Leitung (Pin 1) auf der Platine kennzeichnen.

## Freigabestufen

1. **Entwurf** – Schaltung/Idee, nicht elektrisch geprüft.
2. **Elektrisch geprüft** – ERC/DRC sauber, Netzliste abgeglichen.
3. **Mechanisch geprüft** – Panel, Bauhöhen, Rackschienen kontrolliert.
4. **Prototyp gemessen** – Funktion und Abgleich am realen Aufbau bestätigt.
5. **Fertigungsfreigabe**

ERC/DRC allein belegen weder Funktion noch mechanische Passung.

## Gemeinsame Bibliotheken

Derzeit hat jedes Projekt seine lokalen Bibliotheken (`Serge.kicad_sym`, `Serge_Local.pretty`).
Sobald ein zweites Modul in KiCad entsteht: nach `shared/kicad/` zusammenführen und die lib-tables per `${KIPRJMOD}`-relativem Pfad anpassen.
