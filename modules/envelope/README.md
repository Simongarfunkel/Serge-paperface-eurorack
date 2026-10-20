# Envelope

**Stand:** REV1 elektrisch geprüft (12.10.2026) · **Freigabe:** nein

Vor dem Öffnen: [`hardware/rev1/BITTE_ZUERST_LESEN_REV1.txt`](hardware/rev1/BITTE_ZUERST_LESEN_REV1.txt).

## Revisionen

| Rev | Ordner | Inhalt | Status |
|---|---|---|---|
| REV0 | [`panel/rev0`](panel/rev0) | Original-Panel-DXF, Zeichnungsreferenz, Bilder | **zurückgezogen** – fehlerhafte Angabe zum Stromanschluss; DXF bleibt Panelreferenz |
| REV1 | [`hardware/rev1`](hardware/rev1) | KiCad-Projekt, Gerber, Stückliste, ERC/DRC, Netzabgleich | elektrisch geprüft |

## REV1 in Kürze

- Vollständige Übertragung der 73-75-Envelope-Schaltung, 114 Footprints, beidseitig bestückt.
- Eigener +6-V-Regler aus +12 V, LED-Treiber, isolierte Cycle-Umschaltung, 10-Pin-Eurorack.
- ERC 0, DRC 0, 0 unverbundene Pads, Schaltplan/PCB-Parität 0 Abweichungen.

## Offene Punkte vor Fertigung

- SW1: konkretes Schaltermodell und Bauhöhe bestätigen (Footprint ist generischer Entwurf).
- Mechanischer Gesamtaufbau: Paneldicke, Rackschienenfreiraum, PCB-Umriss 77,28 × 112,5 mm.
- LED-Bohrung (3 mm angenommen; 2,5-mm-Zeichen in der DXF ist nur Positionsmarke).
- Zeitkondensator, Elkos, Trimmer und Teilenummern gegen Datenblätter abgleichen.
- Prototyp: +6 V an TP3 einstellen, Abgleich an TP7, Poti-Wirkrichtung und CV-/Trigger-Funktionen prüfen.

## Quellen

73-75 Build Instructions, S. 32–34; Originalpanel `ENVELOPE_REV.0.dxf`. Weitere im Readme der REV1.
