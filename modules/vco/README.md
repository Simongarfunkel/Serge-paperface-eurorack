# VCO (Oszillator)

**Stand:** Entwurf · **Freigabe:** nein · noch kein KiCad-Projekt

## Dokumente

- [`docs/Serge_73-75_VCO_Originalauszug.pdf`](docs/Serge_73-75_VCO_Originalauszug.pdf) – Originalschaltung, BOM, Trimmanleitung.
- [`docs/Serge_VCO_Stabilisierung_Gruen.pdf`](docs/Serge_VCO_Stabilisierung_Gruen.pdf) – Stabilisierungsvorschlag (16.10.2026, Entwurf, keine freigegebene Nachbauschaltung).

## Original (Kurzfassung)

LM3900-Kern, 3 × 2N3904, 27-nF-Zeitkondensator, drei Trimmer:
1. Initial Offset – tiefste Frequenz, etwa 5–10 Hz
2. Range – Spanne bis etwa 10–14 kHz
3. Sinusformung im Saw-zu-Sinus-Waveshaper

## Geplante Änderungen (laut Vorschlag)

- Konkret: 27 nF als Folie oder C0G/NP0, 100 nF Entkopplung LM3900 Pin 14/7, kurze Timing-Schleife.
- Neu auszulegen: 1-V/Okt.-Eingang mit gepaartem NPN-Expo, Referenzstromregelung, Tempco, gepufferte Präzisionsreferenz.
- Ziel: fünf Oktaven, ±5 Cent nach Warmlaufen – noch nicht nachgewiesen.

## Nächste Schritte

1. Originalkern aufbauen, Strom-/Spannungsbereiche und Reset-Zeit messen.
2. KiCad-Projekt `hardware/rev1` nach Konventionen anlegen.
