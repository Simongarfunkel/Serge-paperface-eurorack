# Gemeinsame KiCad-Bibliotheken

- `Serge.kicad_sym` – Symbole (LM3900 mit Einheiten A–D + Versorgung, Norton-Eingänge, Buchse mit Schaltkontakt, 2N3904/2N3906, Poti, …)
- `Serge_Local.pretty` – Footprints. Übernommen aus Envelope REV1, ergänzt am 22.10.2026:
  - `SOT-23_EBC_MMBT3904` – SOT-23, Padnummern wie Symbol 2N3904 (1=E, 2=B, 3=C) → Pad 2 liegt auf Gehäusepin 1 (B), Pad 1 auf Gehäusepin 2 (E).
  - `D_SOD-123` – 1N4148W, Pad 1 = Kathode.
  - `SOIC-14_3.9x8.7mm_P1.27mm` – LM3900M (Ausnahme VCO).
  - `PinHeader_2x05_P2.54mm_Vertical` – Eurorack-Strom ohne Gehäuse, Pin 1 markiert.
- Einbindung je Projekt über `sym-lib-table` / `fp-lib-table` mit `${KIPRJMOD}/../../../../shared/kicad/…`.
- Envelope REV1 nutzt noch seine lokalen Kopien (unverändert gelassen).

Lizenz der Buchsen-Footprints: `LICENSE_AudioJacks.txt` (MIT).
