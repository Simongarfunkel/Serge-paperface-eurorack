# Bauteilregel (SMD / THT)

Gilt für alle Module ab dem VCO. Vorgabe vom 22.10.2026: **alles SMD, bis auf Potis und Audiobuchsen.**

| Bauteilart | Ausführung | Footprint (Serge_Local) |
|---|---|---|
| Widerstände | SMD | R_0805_2012Metric |
| Keramikkondensatoren | SMD | C_0805_2012Metric (10 µF Entkopplung: X7R 0805/1206) |
| Zeitkonstanten-Kondensatoren (z. B. 27 nF VCO) | SMD C0G/NP0 (1206) | VCO REV1 vorerst Folie THT RM 5 (C_Rect_L7.2mm_W2.5mm_P5.00mm) |
| Elkos | SMD | CP_Elec_5x5.4 (wie Envelope REV1) |
| Dioden 1N4148 → 1N4148W | SMD | D_SOD-123 (Pad 1 = Kathode) |
| Schottky Verpolschutz SS14 | SMD | D_SMA |
| Transistoren 2N3904/2N3906 → MMBT3904/MMBT3906 | SMD | SOT-23_EBC_MMBT3904 (Padnummern wie Symbol: 1=E, 2=B, 3=C) |
| LM3900 → LM3900M | SMD | SOIC-14_3.9x8.7mm_P1.27mm (Verfügbarkeit prüfen) |
| LM741, LM307 → TL071 | SMD | SOIC-8 (Originale abgekündigt) |
| LM1458 → TL072 | SMD | SOIC-8 |
| CA3080 → LM13700 | SMD | SOIC-16, andere Belegung, Schaltung anpassen |
| CA3086 (abgekündigt) | – | gepaarte MMBT3904 oder verfügbares Array; je Modul entscheiden |
| Trimmer 25k / 10k | SMD (z. B. Bourns 3314J) | Footprint noch festlegen; VCO REV1 vorerst 3296W THT |
| Potis 25k linear | THT | Alpha RD901F (Footprint mit Anti-Rotations-Laschen; Ursprung = Pin 1, Achse bei +7,5/+2,5) |
| Buchsen 3,5 mm | THT | Jack_3.5mm_QingPu_WQP-PJ301BM_Vertical |
| Klinke 6,3 mm (Preamp) | THT | noch festlegen |
| RCA (Reverb) | THT | noch festlegen |
| Stromstecker 10-polig | THT (mechanisch) | PinHeader_2x05_P2.54mm_Vertical (ohne Gehäuse; Pin 1 markiert) |

Hinweise
- Die Stückliste jedes Moduls wird aus dem Originalschaltplan abgeleitet, nicht aus der gedruckten BOM. In den
  Build Instructions sind die BOM-Seiten von Triple Waveshaper, Triple Comparator und Positive Slew identisch
  (offensichtlich kopiert) und stimmen nicht mit den Schaltplänen überein.
- Versorgung: ±12 V direkt (Serge V+/V−); +6 V nur, wo die Schaltung es braucht (dann Regler aus +12 V wie Envelope REV1).
- Platine: eine Platine parallel zum Panel, Breite = Panelbreite − 4 mm, Höhe 112,5 mm, Oberkante 8,5 mm unter Panelkante.
  Vorderseite nur Bedienelemente, Rückseite alle anderen Bauteile.
