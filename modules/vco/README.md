# VCO (Oszillator)

**Stand:** REV1 KiCad-Entwurf (22.10.2026), unverdrahtet, ERC/DRC offen · **Freigabe:** nein

## Dokumente

- [`docs/Serge_73-75_VCO_Originalauszug.pdf`](docs/Serge_73-75_VCO_Originalauszug.pdf) – Originalschaltung, BOM, Trimmanleitung.
- [`docs/Schaltplan_Original.png`](docs/Schaltplan_Original.png) – Originalschaltplan als Bild (300 dpi, gedreht).
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

## Revisionen

| Rev | Ordner | Inhalt | Status |
|---|---|---|---|
| REV1 | [`hardware/rev1`](hardware/rev1) | KiCad-Schaltplan (Label-Netzliste), Platine platziert, Stückliste, Netzliste | Entwurf – vor dem Öffnen [`BITTE_ZUERST_LESEN_REV1.txt`](hardware/rev1/BITTE_ZUERST_LESEN_REV1.txt) |

## Nächste Schritte

1. ERC in KiCad, Routing (Freerouting), DRC.
2. Abweichung SUM_P/SH_IN gegen Originalquelle prüfen (siehe BITTE_ZUERST_LESEN).
3. Originalkern aufbauen, Strom-/Spannungsbereiche und Reset-Zeit messen.
