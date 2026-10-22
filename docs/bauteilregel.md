# Bauteilregel (SMD / THT)

Gilt für alle Module ab dem zweiten KiCad-Projekt. Vorgabe vom 21.10.2026.

| Bauteilart | Ausführung | Footprint (Serge_Local / KiCad) |
|---|---|---|
| Widerstände | SMD | R_0805_2012Metric |
| Keramikkondensatoren (pF/nF, Entkopplung) | SMD | C_0805_2012Metric |
| Folienkondensatoren (Zeitkonstanten, z. B. 27 nF, 470 nF, 330 nF) | THT | C_Rect_L7.2mm_W2.5mm_P5.00mm (Wert/Größe prüfen) |
| Elkos | THT | CP_Radial (Durchmesser nach Wert) |
| Dioden 1N4148 | SMD | D_SOD-123 (1N4148W) |
| Transistoren 2N3904/2N3906 | SMD | SOT-23 (MMBT3904/MMBT3906) |
| CA3086 (Transistor-Array) | THT | DIP-14 (nur THT erhältlich) |
| CA3080 (OTA) | THT | DIP-8 (Ersatz LM13700 prüfen) |
| LM3900 | THT | DIP-14_W7.62mm |
| LM741, LM307/TL071, LM1458 | SMD | SOIC-8 (TL071/TL072 als Ersatz) |
| Trimmer 25k / 10k | THT | Potentiometer_Bourns_3296W_Vertical |
| Potis 25k linear | THT | Alpha RD901F (wie Envelope REV1) |
| Buchsen 3,5 mm | THT | Jack_3.5mm_QingPu_WQP-PJ301BM_Vertical |
| Klinke 6,3 mm (Preamp) | THT | noch festlegen |
| RCA (Reverb) | THT | noch festlegen |
| Stromstecker 10-polig | THT | IDC-Header_2x05_P2.54mm_Vertical |

Hinweise
- Die Stückliste jedes Moduls wird aus dem Originalschaltplan abgeleitet, nicht aus der gedruckten BOM. In den
  Build Instructions sind die BOM-Seiten von Triple Waveshaper, Triple Comparator und Positive Slew identisch
  (offensichtlich kopiert) und stimmen nicht mit den Schaltplänen überein.
- +6 V: wie Envelope REV1 eigener Regler aus +12 V je Modul.
