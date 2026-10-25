# Results report — Deep4net\PhysioNet

Generated 2026-10-24 15:24 from the saved `results.json` files. TOST margin ±6 percentage points. Results folder: `<class>/results_session/`.

## 2class

### T1. Test accuracy (%) per subject — chance 50.0%

Protocol: run-wise chronological split per subject: test = the last imagery run of each type (run 12 left/right, run 14 hands/feet); training = runs 4, 8 (and 6, 10); validation = the chronologically last 25% of the training trials of EACH class; refit on all training runs. Subject accuracy = seed ensemble (mean softmax of 3 seeds); single seeds in T6. SD = across subjects (n = 105). Random = mean of the random-montage draws.

| Subject | 64ch | Ours | CSP | RLF | MI | Fixed sensorimotor | ERD-only | Random (mean of draws) |
|---|---|---|---|---|---|---|---|---|
| S01 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 53.33 | 33.33 | 46.67 |
| S02 | 60.00 | 60.00 | 60.00 | 66.67 | 66.67 | 60.00 | 73.33 | 60.00 |
| S03 | 53.33 | 53.33 | 60.00 | 40.00 | 53.33 | 53.33 | 53.33 | 50.67 |
| S04 | 53.33 | 53.33 | 46.67 | 73.33 | 66.67 | 53.33 | 53.33 | 54.67 |
| S05 | 60.00 | 46.67 | 46.67 | 53.33 | 46.67 | 53.33 | 53.33 | 57.33 |
| S06 | 53.33 | 60.00 | 46.67 | 53.33 | 53.33 | 60.00 | 60.00 | 56.00 |
| S07 | 53.33 | 46.67 | 66.67 | 60.00 | 53.33 | 53.33 | 53.33 | 53.33 |
| S08 | 60.00 | 73.33 | 53.33 | 53.33 | 73.33 | 73.33 | 46.67 | 53.33 |
| S09 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 46.67 | 53.33 |
| S10 | 66.67 | 53.33 | 46.67 | 66.67 | 40.00 | 53.33 | 46.67 | 49.33 |
| S11 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 49.33 |
| S12 | 60.00 | 53.33 | 53.33 | 53.33 | 53.33 | 46.67 | 53.33 | 50.67 |
| S13 | 60.00 | 46.67 | 46.67 | 26.67 | 46.67 | 53.33 | 46.67 | 54.67 |
| S14 | 46.67 | 53.33 | 53.33 | 53.33 | 46.67 | 53.33 | 53.33 | 50.67 |
| S15 | 46.67 | 46.67 | 46.67 | 53.33 | 46.67 | 46.67 | 53.33 | 46.67 |
| S16 | 53.33 | 53.33 | 46.67 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 |
| S17 | 53.33 | 53.33 | 73.33 | 53.33 | 60.00 | 66.67 | 53.33 | 60.00 |
| S18 | 53.33 | 46.67 | 53.33 | 53.33 | 60.00 | 60.00 | 53.33 | 52.00 |
| S19 | 53.33 | 40.00 | 40.00 | 33.33 | 33.33 | 53.33 | 33.33 | 46.67 |
| S20 | 66.67 | 60.00 | 46.67 | 46.67 | 60.00 | 40.00 | 46.67 | 54.67 |
| S21 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 |
| S22 | 53.33 | 60.00 | 60.00 | 53.33 | 60.00 | 53.33 | 53.33 | 54.67 |
| S23 | 46.67 | 46.67 | 66.67 | 53.33 | 60.00 | 46.67 | 46.67 | 46.67 |
| S24 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 |
| S25 | 46.67 | 60.00 | 40.00 | 60.00 | 60.00 | 60.00 | 60.00 | 58.67 |
| S26 | 46.67 | 46.67 | 53.33 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 |
| S27 | 40.00 | 46.67 | 33.33 | 53.33 | 46.67 | 40.00 | 46.67 | 48.00 |
| S28 | 66.67 | 40.00 | 53.33 | 53.33 | 53.33 | 66.67 | 66.67 | 52.00 |
| S29 | 53.33 | 46.67 | 46.67 | 46.67 | 53.33 | 80.00 | 60.00 | 52.00 |
| S30 | 60.00 | 66.67 | 53.33 | 53.33 | 60.00 | 66.67 | 66.67 | 66.67 |
| S31 | 53.33 | 40.00 | 53.33 | 66.67 | 60.00 | 53.33 | 66.67 | 60.00 |
| S32 | 66.67 | 46.67 | 60.00 | 53.33 | 66.67 | 60.00 | 80.00 | 60.00 |
| S33 | 46.67 | 46.67 | 46.67 | 53.33 | 53.33 | 66.67 | 46.67 | 48.00 |
| S34 | 53.33 | 46.67 | 46.67 | 46.67 | 46.67 | 53.33 | 46.67 | 48.00 |
| S35 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 |
| S36 | 46.67 | 60.00 | 60.00 | 60.00 | 46.67 | 60.00 | 53.33 | 58.67 |
| S37 | 46.67 | 46.67 | 40.00 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 |
| S38 | 53.33 | 26.67 | 46.67 | 53.33 | 80.00 | 53.33 | 53.33 | 50.67 |
| S39 | 53.33 | 53.33 | 46.67 | 66.67 | 53.33 | 60.00 | 46.67 | 61.33 |
| S40 | 53.33 | 46.67 | 60.00 | 53.33 | 60.00 | 46.67 | 53.33 | 56.00 |
| S41 | 60.00 | 46.67 | 60.00 | 66.67 | 60.00 | 60.00 | 73.33 | 64.00 |
| S42 | 53.33 | 46.67 | 40.00 | 46.67 | 46.67 | 86.67 | 80.00 | 64.00 |
| S43 | 60.00 | 53.33 | 53.33 | 53.33 | 60.00 | 73.33 | 60.00 | 53.33 |
| S44 | 66.67 | 53.33 | 33.33 | 53.33 | 46.67 | 53.33 | 53.33 | 57.33 |
| S45 | 40.00 | 40.00 | 53.33 | 40.00 | 46.67 | 46.67 | 53.33 | 42.67 |
| S46 | 53.33 | 53.33 | 53.33 | 46.67 | 46.67 | 60.00 | 46.67 | 53.33 |
| S47 | 53.33 | 46.67 | 46.67 | 46.67 | 40.00 | 46.67 | 53.33 | 50.67 |
| S48 | 60.00 | 40.00 | 46.67 | 53.33 | 60.00 | 60.00 | 66.67 | 60.00 |
| S49 | 73.33 | 53.33 | 53.33 | 53.33 | 46.67 | 53.33 | 60.00 | 57.33 |
| S50 | 46.67 | 53.33 | 46.67 | 46.67 | 53.33 | 46.67 | 40.00 | 53.33 |
| S51 | 53.33 | 60.00 | 46.67 | 46.67 | 53.33 | 46.67 | 53.33 | 48.00 |
| S52 | 33.33 | 53.33 | 46.67 | 46.67 | 53.33 | 60.00 | 46.67 | 44.00 |
| S53 | 60.00 | 53.33 | 66.67 | 53.33 | 60.00 | 53.33 | 60.00 | 52.00 |
| S54 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 54.67 |
| S55 | 46.67 | 60.00 | 46.67 | 53.33 | 66.67 | 53.33 | 46.67 | 52.00 |
| S56 | 46.67 | 66.67 | 46.67 | 66.67 | 40.00 | 46.67 | 46.67 | 42.67 |
| S57 | 33.33 | 46.67 | 53.33 | 46.67 | 40.00 | 40.00 | 46.67 | 38.67 |
| S58 | 46.67 | 46.67 | 46.67 | 33.33 | 60.00 | 33.33 | 46.67 | 45.33 |
| S59 | 33.33 | 46.67 | 53.33 | 66.67 | 33.33 | 60.00 | 46.67 | 28.00 |
| S60 | 40.00 | 53.33 | 53.33 | 66.67 | 60.00 | 53.33 | 53.33 | 56.00 |
| S61 | 46.67 | 46.67 | 53.33 | 46.67 | 46.67 | 53.33 | 46.67 | 50.67 |
| S62 | 46.67 | 53.33 | 40.00 | 53.33 | 46.67 | 60.00 | 53.33 | 53.33 |
| S63 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 |
| S64 | 53.33 | 46.67 | 53.33 | 46.67 | 60.00 | 53.33 | 46.67 | 56.00 |
| S65 | 46.67 | 46.67 | 53.33 | 46.67 | 46.67 | 33.33 | 46.67 | 45.33 |
| S66 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 66.67 | 53.33 | 53.33 |
| S67 | 46.67 | 46.67 | 46.67 | 73.33 | 60.00 | 46.67 | 46.67 | 54.67 |
| S68 | 53.33 | 46.67 | 60.00 | 40.00 | 46.67 | 53.33 | 53.33 | 45.33 |
| S69 | 66.67 | 53.33 | 46.67 | 53.33 | 60.00 | 60.00 | 53.33 | 53.33 |
| S70 | 60.00 | 53.33 | 60.00 | 53.33 | 60.00 | 60.00 | 53.33 | 54.67 |
| S71 | 66.67 | 53.33 | 53.33 | 46.67 | 53.33 | 53.33 | 60.00 | 57.33 |
| S72 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 |
| S73 | 40.00 | 53.33 | 46.67 | 53.33 | 60.00 | 53.33 | 60.00 | 48.00 |
| S74 | 60.00 | 60.00 | 33.33 | 46.67 | 40.00 | 40.00 | 46.67 | 46.67 |
| S75 | 46.67 | 46.67 | 53.33 | 53.33 | 53.33 | 46.67 | 46.67 | 44.00 |
| S76 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 |
| S77 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 60.00 | 60.00 | 48.00 |
| S78 | 53.33 | 53.33 | 60.00 | 53.33 | 53.33 | 60.00 | 53.33 | 53.33 |
| S79 | 40.00 | 40.00 | 53.33 | 46.67 | 46.67 | 60.00 | 46.67 | 54.67 |
| S80 | 53.33 | 40.00 | 53.33 | 53.33 | 46.67 | 40.00 | 53.33 | 49.33 |
| S81 | 66.67 | 53.33 | 60.00 | 53.33 | 53.33 | 53.33 | 53.33 | 57.33 |
| S82 | 46.67 | 46.67 | 66.67 | 46.67 | 46.67 | 60.00 | 53.33 | 46.67 |
| S83 | 60.00 | 53.33 | 53.33 | 46.67 | 53.33 | 53.33 | 53.33 | 53.33 |
| S84 | 40.00 | 46.67 | 40.00 | 73.33 | 73.33 | 53.33 | 46.67 | 54.67 |
| S85 | 46.67 | 46.67 | 60.00 | 53.33 | 60.00 | 66.67 | 60.00 | 61.33 |
| S86 | 46.67 | 46.67 | 80.00 | 46.67 | 46.67 | 53.33 | 46.67 | 46.67 |
| S87 | 53.33 | 53.33 | 53.33 | 60.00 | 60.00 | 60.00 | 40.00 | 50.67 |
| S89 | 46.67 | 60.00 | 33.33 | 66.67 | 33.33 | 53.33 | 46.67 | 50.67 |
| S90 | 46.67 | 46.67 | 33.33 | 40.00 | 40.00 | 33.33 | 53.33 | 36.00 |
| S91 | 53.33 | 53.33 | 80.00 | 53.33 | 66.67 | 53.33 | 46.67 | 61.33 |
| S93 | 53.33 | 46.67 | 53.33 | 46.67 | 46.67 | 46.67 | 46.67 | 53.33 |
| S94 | 66.67 | 73.33 | 53.33 | 66.67 | 66.67 | 66.67 | 60.00 | 62.67 |
| S95 | 46.67 | 46.67 | 26.67 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 |
| S96 | 53.33 | 53.33 | 53.33 | 46.67 | 53.33 | 53.33 | 46.67 | 50.67 |
| S97 | 66.67 | 66.67 | 53.33 | 60.00 | 66.67 | 80.00 | 53.33 | 60.00 |
| S98 | 60.00 | 33.33 | 53.33 | 40.00 | 53.33 | 33.33 | 60.00 | 53.33 |
| S99 | 40.00 | 40.00 | 46.67 | 33.33 | 53.33 | 33.33 | 40.00 | 37.33 |
| S101 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 |
| S102 | 46.67 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 | 53.33 |
| S103 | 40.00 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 60.00 | 48.00 |
| S105 | 53.33 | 60.00 | 46.67 | 53.33 | 53.33 | 40.00 | 46.67 | 50.67 |
| S106 | 53.33 | 53.33 | 60.00 | 46.67 | 40.00 | 60.00 | 66.67 | 60.00 |
| S107 | 46.67 | 40.00 | 40.00 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 |
| S108 | 53.33 | 60.00 | 60.00 | 66.67 | 66.67 | 46.67 | 66.67 | 50.67 |
| S109 | 33.33 | 46.67 | 46.67 | 46.67 | 46.67 | 46.67 | 40.00 | 42.67 |
| Mean | 52.06 | 50.79 | 51.30 | 52.13 | 52.95 | 53.65 | 52.51 | 51.82 |
| SD | 8.17 | 7.36 | 8.83 | 8.46 | 8.61 | 9.58 | 8.20 | 6.21 |

### T2. Montages and profiles

Full list per subject in `T2_montages.csv` (all 12-channel montages are leave-one-subject-out).

| Method | Distinct montages across subjects | Most frequent montage |
|---|---|---|
| Ours | 82 | FC6 TP8 C4 CP4 C6 FT8 F8 F4 FC4 F5 PO8 P6 |
| CSP | 15 | Fpz Fp1 AF7 Fp2 AFz AF3 AF8 AF4 F8 F7 F5 F1 |
| RLF | 70 | F7 CP6 C4 CP4 FT7 F8 P6 C6 P4 T9 FC4 PO4 |
| MI | 94 | F7 F8 F5 P6 F2 F3 FC4 CP4 CP6 CP2 P4 F4 |
| Fixed sensorimotor | 1 | FC3 FC1 FC2 FC4 C3 C1 Cz C2 C4 CP3 CPz CP4 |
| ERD-only | 8 | PO8 O2 O1 PO4 Oz POz PO7 PO3 Fpz P4 P2 Fp2 |

### T3. Equivalence of each 12-channel montage with all 64 channels (paired TOST)

Difference = montage − 64ch, in percentage points. Equivalent means the 90% CI lies inside the margin; it does not mean identical accuracy.

| Method | n | Mean diff (pp) | SD | 90% CI | TOST p | Equivalent (±6 pp) | Worst subject (pp) | Subjects losing >6 pp | Equivalent at margins (pp) |
|---|---|---|---|---|---|---|---|---|---|
| Ours | 105 | -1.27 | 9.34 | [-2.78, +0.24] | <0.0001 | yes | -26.67 | 34 | 3,4,5,6,8,10 |
| CSP | 105 | -0.76 | 11.07 | [-2.55, +1.03] | <0.0001 | yes | -33.33 | 41 | 3,4,5,6,8,10 |
| RLF | 105 | +0.06 | 11.23 | [-1.76, +1.88] | <0.0001 | yes | -33.33 | 37 | 2,3,4,5,6,8,10 |
| MI | 105 | +0.89 | 10.13 | [-0.75, +2.53] | <0.0001 | yes | -26.67 | 26 | 3,4,5,6,8,10 |
| Fixed sensorimotor | 105 | +1.59 | 10.68 | [-0.14, +3.32] | <0.0001 | yes | -26.67 | 26 | 4,5,6,8,10 |
| ERD-only | 105 | +0.44 | 8.88 | [-0.99, +1.88] | <0.0001 | yes | -20.00 | 29 | 2,3,4,5,6,8,10 |
| Random (mean of draws) | 105 | -0.24 | 6.82 | [-1.35, +0.86] | <0.0001 | yes | -17.33 | 20 | 2,3,4,5,6,8,10 |

### T4. Saliency montage (Ours) vs every other 12-channel montage

Positive = Ours more accurate. Holm correction across the comparisons in this table.

| Ours vs | n | Mean diff (pp) | 95% CI | paired t p | Holm | Wilcoxon p | Holm | Ours better / tie / worse |
|---|---|---|---|---|---|---|---|---|
| CSP | 105 | -0.51 | [-2.67, +1.65] | 0.6419 | 0.6419 | 0.7605 | 0.9316 | 29 / 41 / 35 |
| RLF | 105 | -1.33 | [-3.08, +0.41] | 0.1333 | 0.3999 | 0.2395 | 0.9316 | 25 / 49 / 31 |
| MI | 105 | -2.16 | [-4.13, -0.19] | 0.0322 | 0.1611 | 0.0312 | 0.1558 | 21 / 47 / 37 |
| Fixed sensorimotor | 105 | -2.86 | [-4.84, -0.87] | 0.0052 | 0.0310 | 0.0140 | 0.0838 | 18 / 46 / 41 |
| ERD-only | 105 | -1.71 | [-3.76, +0.33] | 0.0999 | 0.3998 | 0.2603 | 0.9316 | 24 / 48 / 33 |
| Random (mean of draws) | 105 | -1.03 | [-2.59, +0.54] | 0.1950 | 0.3999 | 0.2329 | 0.9316 | 35 / 28 / 42 |

### T5. Confusion, class balance and majority baseline (chance 50.0%)

Pooled over all subjects, folds and seeds; full matrices in `T5_confusion_matrices.csv`. The last column flags models that collapsed to one class.

| Method | Pooled acc | Per-class recall | Predicted share per class | Mean majority-class acc | Folds predicting one class ≥90% |
|---|---|---|---|---|---|
| 64ch | 52.06 | left_hand 54.9, right_hand 49.2 | left_hand 52.8, right_hand 47.2 | 53.33 | 55 / 105 |
| Ours | 50.79 | left_hand 64.6, right_hand 36.8 | left_hand 63.9, right_hand 36.1 | 53.33 | 71 / 105 |
| CSP | 51.30 | left_hand 49.4, right_hand 53.2 | left_hand 48.1, right_hand 51.9 | 53.33 | 46 / 105 |
| RLF | 52.13 | left_hand 54.0, right_hand 50.3 | left_hand 51.9, right_hand 48.1 | 53.33 | 61 / 105 |
| MI | 52.95 | left_hand 58.1, right_hand 47.7 | left_hand 55.2, right_hand 44.8 | 53.33 | 57 / 105 |
| Fixed sensorimotor | 53.65 | left_hand 57.0, right_hand 50.3 | left_hand 53.4, right_hand 46.6 | 53.33 | 53 / 105 |
| ERD-only | 52.51 | left_hand 56.2, right_hand 48.7 | left_hand 53.8, right_hand 46.2 | 53.33 | 60 / 105 |
| Random (mean of draws) | 51.82 | left_hand 53.3, right_hand 50.4 | left_hand 51.5, right_hand 48.5 | 53.33 | 297 / 525 |

### T6. Seed stability

Grand mean of each single seed, before the seed ensemble used in T1.

| Method | Seeds | Grand mean per seed (%) | Mean across seeds | SD across seeds |
|---|---|---|---|---|
| 64ch | 3 | 42: 52.32, 43: 53.21, 44: 52.19 | 52.57 | 0.55 |
| Ours | 3 | 42: 51.81, 43: 50.79, 44: 50.86 | 51.15 | 0.57 |
| CSP | 3 | 42: 50.98, 43: 52.06, 44: 51.75 | 51.60 | 0.55 |
| RLF | 3 | 42: 51.17, 43: 50.41, 44: 52.38 | 51.32 | 0.99 |
| MI | 3 | 42: 51.81, 43: 51.68, 44: 51.24 | 51.58 | 0.30 |
| Fixed sensorimotor | 3 | 42: 51.87, 43: 52.63, 44: 53.21 | 52.57 | 0.67 |
| ERD-only | 3 | 42: 52.25, 43: 52.25, 44: 51.75 | 52.08 | 0.29 |
| Random (mean of draws) | 3 | 42: 51.92, 43: 51.54, 44: 51.17 | 51.55 | 0.37 |

### T7. Saliency vs ERD/ERS alignment (participant level)

magnitude / class_specific / lateralisation compare unsigned saliency with desynchronisation strength (−ERD) and are sign-invariant; `legacy_signed_LR` is the old statistic, shown only for comparison (its sign is not interpretable). Mean and CI via Fisher z. Per-subject values: `results/full64/alignment_metrics.json`.

| Attribution | Metric | Mean r (Fisher) | 95% CI | SD of r | n subjects |
|---|---|---|---|---|---|
| grad | magnitude_pearson | 0.016 | [-0.032, 0.064] | 0.231 | 105 |
| grad | class_specific_pearson | 0.002 | [-0.040, 0.044] | 0.204 | 105 |
| grad | lateralisation_pearson | -0.033 | [-0.068, 0.002] | 0.176 | 105 |
| grad | magnitude_spearman | -0.001 | [-0.049, 0.047] | 0.230 | 105 |
| grad | class_specific_spearman | 0.009 | [-0.033, 0.050] | 0.199 | 105 |
| grad | lateralisation_spearman | -0.033 | [-0.069, 0.003] | 0.179 | 105 |
| grad | legacy_signed_LR_pearson | -0.023 | [-0.078, 0.033] | 0.263 | 105 |
| grad_x_input | magnitude_pearson | -0.025 | [-0.092, 0.042] | 0.305 | 105 |
| grad_x_input | class_specific_pearson | -0.005 | [-0.062, 0.053] | 0.272 | 105 |
| grad_x_input | lateralisation_pearson | -0.143 | [-0.231, -0.053] | 0.397 | 105 |
| grad_x_input | magnitude_spearman | -0.032 | [-0.096, 0.031] | 0.290 | 105 |
| grad_x_input | class_specific_spearman | -0.006 | [-0.062, 0.051] | 0.264 | 105 |
| grad_x_input | lateralisation_spearman | -0.137 | [-0.220, -0.052] | 0.381 | 105 |
| grad_x_input | legacy_signed_LR_pearson | -0.059 | [-0.128, 0.011] | 0.328 | 105 |
| integrated_gradients | magnitude_pearson | -0.029 | [-0.096, 0.037] | 0.307 | 105 |
| integrated_gradients | class_specific_pearson | -0.010 | [-0.066, 0.045] | 0.264 | 105 |
| integrated_gradients | lateralisation_pearson | -0.159 | [-0.246, -0.070] | 0.398 | 105 |
| integrated_gradients | magnitude_spearman | -0.036 | [-0.098, 0.027] | 0.290 | 105 |
| integrated_gradients | class_specific_spearman | -0.010 | [-0.065, 0.044] | 0.257 | 105 |
| integrated_gradients | lateralisation_spearman | -0.146 | [-0.229, -0.061] | 0.383 | 105 |
| integrated_gradients | legacy_signed_LR_pearson | -0.057 | [-0.126, 0.013] | 0.327 | 105 |
| smoothgrad | magnitude_pearson | 0.015 | [-0.033, 0.063] | 0.231 | 105 |
| smoothgrad | class_specific_pearson | 0.003 | [-0.039, 0.046] | 0.205 | 105 |
| smoothgrad | lateralisation_pearson | -0.036 | [-0.073, 0.000] | 0.184 | 105 |
| smoothgrad | magnitude_spearman | -0.001 | [-0.050, 0.047] | 0.232 | 105 |
| smoothgrad | class_specific_spearman | 0.009 | [-0.033, 0.050] | 0.200 | 105 |
| smoothgrad | lateralisation_spearman | -0.036 | [-0.074, 0.001] | 0.187 | 105 |
| smoothgrad | legacy_signed_LR_pearson | -0.021 | [-0.077, 0.035] | 0.263 | 105 |

### T7b. Correlations as computed by the original scripts

corr(saliency, ERD_L / ERD_R / ERD_(L−R) / ERD_comb) and corr(saliency, plain-gradient saliency), participant level. Kept so the earlier numbers can be compared; an unsigned map is correlated with a signed one, so the sign is not 'agreement' (use T7).

| Attribution | Correlation | Mean r (Fisher) | 95% CI | n subjects |
|---|---|---|---|---|
| grad | ERD_L_pearson | -0.027 | [-0.082, 0.028] | 105 |
| grad | ERD_L_spearman | -0.031 | [-0.087, 0.026] | 105 |
| grad | ERD_R_pearson | 0.018 | [-0.037, 0.072] | 105 |
| grad | ERD_R_spearman | 0.004 | [-0.049, 0.057] | 105 |
| grad | ERD_LR_pearson | -0.023 | [-0.078, 0.033] | 105 |
| grad | ERD_LR_spearman | -0.006 | [-0.063, 0.051] | 105 |
| grad | ERD_comb_pearson | -0.002 | [-0.056, 0.053] | 105 |
| grad | ERD_comb_spearman | -0.015 | [-0.072, 0.042] | 105 |
| grad | vs_grad_pearson | 1.000 | [1.000, 1.000] | 105 |
| grad | vs_grad_spearman | 1.000 | [1.000, 1.000] | 105 |
| grad_x_input | ERD_L_pearson | -0.068 | [-0.139, 0.004] | 105 |
| grad_x_input | ERD_L_spearman | -0.057 | [-0.129, 0.016] | 105 |
| grad_x_input | ERD_R_pearson | 0.022 | [-0.054, 0.097] | 105 |
| grad_x_input | ERD_R_spearman | 0.020 | [-0.053, 0.093] | 105 |
| grad_x_input | ERD_LR_pearson | -0.059 | [-0.128, 0.011] | 105 |
| grad_x_input | ERD_LR_spearman | -0.044 | [-0.112, 0.026] | 105 |
| grad_x_input | ERD_comb_pearson | -0.035 | [-0.108, 0.039] | 105 |
| grad_x_input | ERD_comb_spearman | -0.020 | [-0.093, 0.054] | 105 |
| grad_x_input | vs_grad_pearson | 0.781 | [0.741, 0.816] | 105 |
| grad_x_input | vs_grad_spearman | 0.778 | [0.743, 0.809] | 105 |
| integrated_gradients | ERD_L_pearson | -0.068 | [-0.140, 0.005] | 105 |
| integrated_gradients | ERD_L_spearman | -0.064 | [-0.137, 0.010] | 105 |
| integrated_gradients | ERD_R_pearson | 0.029 | [-0.044, 0.102] | 105 |
| integrated_gradients | ERD_R_spearman | 0.016 | [-0.056, 0.088] | 105 |
| integrated_gradients | ERD_LR_pearson | -0.057 | [-0.126, 0.013] | 105 |
| integrated_gradients | ERD_LR_spearman | -0.041 | [-0.110, 0.028] | 105 |
| integrated_gradients | ERD_comb_pearson | -0.029 | [-0.102, 0.043] | 105 |
| integrated_gradients | ERD_comb_spearman | -0.025 | [-0.097, 0.048] | 105 |
| integrated_gradients | vs_grad_pearson | 0.776 | [0.736, 0.811] | 105 |
| integrated_gradients | vs_grad_spearman | 0.771 | [0.735, 0.802] | 105 |
| smoothgrad | ERD_L_pearson | -0.027 | [-0.082, 0.028] | 105 |
| smoothgrad | ERD_L_spearman | -0.031 | [-0.087, 0.026] | 105 |
| smoothgrad | ERD_R_pearson | 0.016 | [-0.039, 0.070] | 105 |
| smoothgrad | ERD_R_spearman | 0.003 | [-0.049, 0.056] | 105 |
| smoothgrad | ERD_LR_pearson | -0.021 | [-0.077, 0.035] | 105 |
| smoothgrad | ERD_LR_spearman | -0.005 | [-0.062, 0.052] | 105 |
| smoothgrad | ERD_comb_pearson | -0.003 | [-0.058, 0.052] | 105 |
| smoothgrad | ERD_comb_spearman | -0.016 | [-0.073, 0.041] | 105 |
| smoothgrad | vs_grad_pearson | 0.999 | [0.999, 0.999] | 105 |
| smoothgrad | vs_grad_spearman | 0.998 | [0.997, 0.998] | 105 |

### T10. EXPLORATORY: saliency vs other physiological maps

Curiosity only — not used for any choice; the paper's alignment is T7. Saliency = mean of the four attribution maps (`mean4`); per method in `T10_physiology_all_methods.csv`. r = corr(saliency, map), |map| = corr(saliency, |map|), class-specific = mean of corr(saliency_L, |map_L|) and corr(saliency_R, |map_R|). Fisher-z mean over subjects. Group maps: `figures/physiology_maps_group.png`.

| Map | Pearson r | 95% CI | Pearson r (|map|) | Spearman r | Spearman r (|map|) | n |
|---|---|---|---|---|---|---|
| ERD_theta_L | -0.090 | [-0.162, -0.017] | -0.085 | -0.075 | -0.059 | 105 |
| ERD_theta_R | -0.038 | [-0.113, 0.037] | -0.049 | -0.038 | -0.043 | 105 |
| ERD_theta_mag | -0.097 | [-0.166, -0.027] | -0.097 | -0.070 | -0.070 | 105 |
| ERD_mu_L | -0.059 | [-0.121, 0.003] | -0.018 | -0.051 | -0.024 | 105 |
| ERD_mu_R | 0.003 | [-0.063, 0.069] | -0.003 | 0.002 | -0.005 | 105 |
| ERD_mu_mag | -0.010 | [-0.066, 0.047] | -0.010 | -0.023 | -0.023 | 105 |
| ERD_beta_L | -0.033 | [-0.094, 0.028] | 0.000 | -0.034 | 0.012 | 105 |
| ERD_beta_R | 0.029 | [-0.030, 0.087] | -0.049 | 0.022 | -0.045 | 105 |
| ERD_beta_mag | -0.038 | [-0.086, 0.011] | -0.038 | -0.025 | -0.025 | 105 |
| ERS_beta_rebound_L | -0.014 | [-0.069, 0.042] | 0.044 | -0.006 | 0.050 | 105 |
| ERS_beta_rebound_R | -0.013 | [-0.073, 0.048] | -0.025 | -0.018 | -0.025 | 105 |
| ERS_beta_rebound_mag | 0.017 | [-0.035, 0.069] | 0.017 | 0.018 | 0.018 | 105 |
| ERD_lowgamma_L | -0.024 | [-0.078, 0.030] | -0.014 | -0.031 | -0.026 | 105 |
| ERD_lowgamma_R | -0.024 | [-0.076, 0.028] | 0.011 | -0.021 | 0.009 | 105 |
| ERD_lowgamma_mag | -0.004 | [-0.053, 0.044] | -0.004 | -0.009 | -0.009 | 105 |
| logpow_8_30 | 0.034 | [-0.016, 0.085] | 0.034 | 0.019 | 0.019 | 105 |
| r2_signed | 0.063 | [0.000, 0.126] | 0.028 | 0.058 | 0.025 | 105 |
| r2_abs | 0.028 | [-0.031, 0.087] | 0.028 | 0.025 | 0.025 | 105 |
| TFR_ERD_dB_L | -0.060 | [-0.123, 0.004] | -0.014 | -0.062 | -0.006 | 105 |
| TFR_ERD_dB_R | 0.005 | [-0.057, 0.066] | -0.053 | -0.004 | -0.053 | 105 |
| TFR_ERD_dB_mag | -0.043 | [-0.096, 0.010] | -0.043 | -0.036 | -0.036 | 105 |
| ITC_4_30 | -0.003 | [-0.053, 0.048] | -0.003 | -0.001 | -0.001 | 105 |
| ERP_abs_0.2_0.8 | -0.077 | [-0.143, -0.011] | -0.077 | -0.053 | -0.053 | 105 |
| SlowPot_0.5_3 | -0.021 | [-0.085, 0.043] | -0.058 | -0.020 | -0.041 | 105 |
| ERD_beta_classspecific | — | — | -0.014 [-0.049, 0.020] | — | -0.006 | 105 |
| ERD_lowgamma_classspecific | — | — | 0.001 [-0.033, 0.036] | — | -0.004 | 105 |
| ERD_mu_classspecific | — | — | -0.009 [-0.049, 0.032] | — | -0.012 | 105 |
| ERD_theta_classspecific | — | — | -0.069 [-0.122, -0.017] | — | -0.055 | 105 |
| ERS_beta_rebound_classspecific | — | — | 0.008 [-0.027, 0.044] | — | 0.015 | 105 |
| TFR_ERD_dB_classspecific | — | — | -0.022 [-0.059, 0.016] | — | -0.017 | 105 |

### T8a. Faithfulness: deletion test on the test trials

Accuracy drop (intact − channels removed), mean ± SD across subjects. Ranking from validation saliency; removal = channel set to its standardised mean. A faithful ranking gives the largest drop for top-ranked channels.

| Removed channels k | Drop: top-ranked (pp) | Drop: random (pp) | Drop: bottom-ranked (pp) | top vs random p | top vs bottom p |
|---|---|---|---|---|---|
| 2 | +0.11 ± 1.91 | +0.18 ± 1.38 | +0.17 ± 1.50 | 0.5705 | 0.7074 |
| 4 | +0.02 ± 2.64 | +0.31 ± 1.89 | +0.34 ± 2.06 | 0.0983 | 0.1739 |
| 6 | +0.11 ± 3.18 | +0.29 ± 2.48 | +0.32 ± 2.49 | 0.3499 | 0.4430 |

### T8b. Model-randomisation sanity check

Similarity between saliency of the trained model and of an untrained model. High values mean the map reflects the input more than what the network learned.

| Attribution | Spearman(trained, untrained model) | 95% CI | n subjects |
|---|---|---|---|
| grad | -0.013 | [-0.027, 0.001] | 105 |
| grad_x_input | 0.333 | [0.290, 0.375] | 105 |
| integrated_gradients | 0.331 | [0.287, 0.373] | 105 |
| smoothgrad | -0.013 | [-0.026, 0.001] | 105 |

### T9. Configuration

Full snapshot: `T9_config.json`.

Training profile chosen on validation data only, leave-one-subject-out (unanimous: True): S01=zscore, S02=zscore, S03=zscore, S04=zscore, S05=zscore, S06=zscore, S07=zscore, S08=zscore, S09=zscore, S10=zscore, S11=zscore, S12=zscore, S13=zscore, S14=zscore, S15=zscore, S16=zscore, S17=zscore, S18=zscore, S19=zscore, S20=zscore, S21=zscore, S22=zscore, S23=zscore, S24=zscore, S25=zscore, S26=zscore, S27=zscore, S28=zscore, S29=zscore, S30=zscore, S31=zscore, S32=zscore, S33=zscore, S34=zscore, S35=zscore, S36=zscore, S37=zscore, S38=zscore, S39=zscore, S40=zscore, S41=zscore, S42=zscore, S43=zscore, S44=zscore, S45=zscore, S46=zscore, S47=zscore, S48=zscore, S49=zscore, S50=zscore, S51=zscore, S52=zscore, S53=zscore, S54=zscore, S55=zscore, S56=zscore, S57=zscore, S58=zscore, S59=zscore, S60=zscore, S61=zscore, S62=zscore, S63=zscore, S64=zscore, S65=zscore, S66=zscore, S67=zscore, S68=zscore, S69=zscore, S70=zscore, S71=zscore, S72=zscore, S73=zscore, S74=zscore, S75=zscore, S76=zscore, S77=zscore, S78=zscore, S79=zscore, S80=zscore, S81=zscore, S82=zscore, S83=zscore, S84=zscore, S85=zscore, S86=zscore, S87=zscore, S89=zscore, S90=zscore, S91=zscore, S93=zscore, S94=zscore, S95=zscore, S96=zscore, S97=zscore, S98=zscore, S99=zscore, S101=zscore, S102=zscore, S103=zscore, S105=zscore, S106=zscore, S107=zscore, S108=zscore, S109=zscore

| Profile | Mean validation accuracy (%) |
|---|---|
| zscore | 65.36 |
| ems | 63.93 |
| original | 50.00 |

```
model: "Deep4Net"
dataset: "PhysionetMI"
sfreq_hz: "per profile (profiles[*].sfreq)"
profiles: {"zscore": {"sfreq": 160, "band_hz": [4.0, 40.0], "window_s": [0.0, 3.0], "car": false, "norm": null, "align": "zscore", "dropout": 0.5, "pool_time_length": 3, "pool_time_stride": 3, "lr": 0.001, "weight_decay": 0.0005, "scheduler": "cosine", "max_epochs": 300, "patience": 80, "batch_size": 16, "label_smoothing": 0.1, "grad_clip": 10.0, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "ems": {"sfreq": 160, "band_hz": [4.0, 40.0], "window_s": [0.0, 3.0], "car": false, "norm": "ems", "align": null, "dropout": 0.5, "pool_time_length": 3, "pool_time_stride": 3, "lr": 0.001, "weight_decay": 0.0005, "scheduler": "cosine", "max_epochs": 300, "patience": 80, "batch_size": 16, "label_smoothing": 0.1, "grad_clip": 10.0, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "original": {"sfreq": 160, "band_hz": [8.0, 32.0], "window_s": [0.5, 2.5], "norm": null, "align": null, "car": false, "dropout": 0.25, "pool_time_length": 2, "pool_time_stride": 2, "lr": 0.01, "weight_decay": 1e-05, "scheduler": "multistep", "milestones": [20, 50], "gamma": 0.1, "max_epochs": 100, "patience": 100, "batch_size": 64, "label_smoothing": 0.0, "grad_clip": 10.0, "augment": false, "select_on": "val_loss", "min_select_epoch": 1}}
checkpoint_rule: "highest validation accuracy (loss breaks ties), not before epoch 20 ('original': lowest validation loss); refit keeps the final weights"
folds: "run-wise chronological split per subject: test = the last imagery run of each type (run 12 left/right, run 14 hands/feet); training = runs 4, 8 (and 6, 10); validation = the chronologically last 25% of the training trials of EACH class; refit on all training runs"
seeds: [42, 43, 44]
```

Figures (530 topomaps: saliency per method/subject, group maps, ERD/ERS) copied to `2class\figures`.

## 4class

### T1. Test accuracy (%) per subject — chance 25.0%

Protocol: run-wise chronological split per subject: test = the last imagery run of each type (run 12 left/right, run 14 hands/feet); training = runs 4, 8 (and 6, 10); validation = the chronologically last 25% of the training trials of EACH class; refit on all training runs. Subject accuracy = seed ensemble (mean softmax of 3 seeds); single seeds in T6. SD = across subjects (n = 105). Random = mean of the random-montage draws.

| Subject | 64ch | Ours | CSP | RLF | MI | Fixed sensorimotor | ERD-only | Random (mean of draws) |
|---|---|---|---|---|---|---|---|---|
| S01 | 20.00 | 23.33 | 23.33 | 6.67 | 10.00 | 26.67 | 26.67 | 27.33 |
| S02 | 36.67 | 53.33 | 40.00 | 43.33 | 30.00 | 30.00 | 43.33 | 43.33 |
| S03 | 30.00 | 36.67 | 33.33 | 40.00 | 30.00 | 43.33 | 33.33 | 40.67 |
| S04 | 26.67 | 20.00 | 26.67 | 23.33 | 26.67 | 30.00 | 23.33 | 27.33 |
| S05 | 20.00 | 30.00 | 23.33 | 30.00 | 26.67 | 23.33 | 23.33 | 25.33 |
| S06 | 23.33 | 23.33 | 20.00 | 26.67 | 20.00 | 30.00 | 26.67 | 28.00 |
| S07 | 30.00 | 36.67 | 26.67 | 30.00 | 26.67 | 33.33 | 43.33 | 30.00 |
| S08 | 23.33 | 30.00 | 23.33 | 30.00 | 30.00 | 26.67 | 20.00 | 26.00 |
| S09 | 20.00 | 23.33 | 23.33 | 23.33 | 6.67 | 30.00 | 23.33 | 19.33 |
| S10 | 30.00 | 36.67 | 30.00 | 36.67 | 36.67 | 13.33 | 26.67 | 21.33 |
| S11 | 30.00 | 30.00 | 26.67 | 26.67 | 23.33 | 26.67 | 30.00 | 26.67 |
| S12 | 30.00 | 26.67 | 30.00 | 33.33 | 30.00 | 23.33 | 23.33 | 32.67 |
| S13 | 26.67 | 33.33 | 23.33 | 23.33 | 26.67 | 33.33 | 26.67 | 24.00 |
| S14 | 23.33 | 23.33 | 26.67 | 26.67 | 36.67 | 20.00 | 26.67 | 24.67 |
| S15 | 26.67 | 36.67 | 40.00 | 30.00 | 26.67 | 30.00 | 40.00 | 32.00 |
| S16 | 30.00 | 30.00 | 26.67 | 36.67 | 33.33 | 23.33 | 36.67 | 32.67 |
| S17 | 30.00 | 26.67 | 30.00 | 30.00 | 30.00 | 30.00 | 26.67 | 30.00 |
| S18 | 40.00 | 30.00 | 40.00 | 56.67 | 50.00 | 30.00 | 33.33 | 40.67 |
| S19 | 33.33 | 33.33 | 30.00 | 23.33 | 36.67 | 30.00 | 30.00 | 30.67 |
| S20 | 33.33 | 33.33 | 30.00 | 30.00 | 40.00 | 30.00 | 33.33 | 32.00 |
| S21 | 23.33 | 23.33 | 23.33 | 23.33 | 23.33 | 23.33 | 23.33 | 24.00 |
| S22 | 26.67 | 30.00 | 30.00 | 30.00 | 23.33 | 26.67 | 30.00 | 28.00 |
| S23 | 26.67 | 23.33 | 20.00 | 26.67 | 23.33 | 26.67 | 26.67 | 30.00 |
| S24 | 26.67 | 23.33 | 30.00 | 26.67 | 30.00 | 23.33 | 26.67 | 28.67 |
| S25 | 23.33 | 26.67 | 20.00 | 26.67 | 23.33 | 26.67 | 20.00 | 22.00 |
| S26 | 33.33 | 23.33 | 30.00 | 23.33 | 26.67 | 26.67 | 30.00 | 28.67 |
| S27 | 26.67 | 40.00 | 20.00 | 30.00 | 30.00 | 23.33 | 26.67 | 27.33 |
| S28 | 16.67 | 46.67 | 23.33 | 43.33 | 40.00 | 20.00 | 33.33 | 25.33 |
| S29 | 50.00 | 33.33 | 13.33 | 26.67 | 36.67 | 23.33 | 26.67 | 37.33 |
| S30 | 30.00 | 33.33 | 30.00 | 40.00 | 33.33 | 33.33 | 43.33 | 36.00 |
| S31 | 33.33 | 23.33 | 20.00 | 30.00 | 33.33 | 33.33 | 43.33 | 29.33 |
| S32 | 10.00 | 3.33 | 16.67 | 6.67 | 6.67 | 10.00 | 16.67 | 8.67 |
| S33 | 30.00 | 30.00 | 6.67 | 26.67 | 33.33 | 36.67 | 20.00 | 33.33 |
| S34 | 30.00 | 43.33 | 33.33 | 33.33 | 36.67 | 30.00 | 26.67 | 34.00 |
| S35 | 50.00 | 56.67 | 40.00 | 43.33 | 56.67 | 50.00 | 53.33 | 46.00 |
| S36 | 30.00 | 20.00 | 16.67 | 20.00 | 16.67 | 26.67 | 20.00 | 23.33 |
| S37 | 20.00 | 26.67 | 26.67 | 26.67 | 26.67 | 20.00 | 26.67 | 24.67 |
| S38 | 20.00 | 3.33 | 23.33 | 16.67 | 3.33 | 26.67 | 26.67 | 22.67 |
| S39 | 13.33 | 16.67 | 30.00 | 30.00 | 23.33 | 26.67 | 23.33 | 24.00 |
| S40 | 33.33 | 20.00 | 26.67 | 26.67 | 26.67 | 30.00 | 33.33 | 29.33 |
| S41 | 33.33 | 53.33 | 26.67 | 53.33 | 56.67 | 26.67 | 30.00 | 36.67 |
| S42 | 46.67 | 33.33 | 33.33 | 36.67 | 40.00 | 63.33 | 30.00 | 41.33 |
| S43 | 16.67 | 16.67 | 16.67 | 16.67 | 13.33 | 20.00 | 33.33 | 19.33 |
| S44 | 36.67 | 26.67 | 26.67 | 20.00 | 20.00 | 26.67 | 36.67 | 30.67 |
| S45 | 40.00 | 43.33 | 30.00 | 50.00 | 43.33 | 40.00 | 33.33 | 38.00 |
| S46 | 23.33 | 26.67 | 16.67 | 23.33 | 23.33 | 30.00 | 23.33 | 19.33 |
| S47 | 13.33 | 16.67 | 26.67 | 23.33 | 30.00 | 20.00 | 10.00 | 17.33 |
| S48 | 40.00 | 30.00 | 26.67 | 26.67 | 36.67 | 40.00 | 40.00 | 48.00 |
| S49 | 36.67 | 20.00 | 20.00 | 23.33 | 33.33 | 20.00 | 33.33 | 30.67 |
| S50 | 33.33 | 20.00 | 10.00 | 26.67 | 23.33 | 20.00 | 30.00 | 24.00 |
| S51 | 26.67 | 30.00 | 43.33 | 46.67 | 40.00 | 30.00 | 26.67 | 33.33 |
| S52 | 46.67 | 40.00 | 33.33 | 20.00 | 26.67 | 26.67 | 36.67 | 31.33 |
| S53 | 33.33 | 36.67 | 36.67 | 33.33 | 36.67 | 26.67 | 20.00 | 26.67 |
| S54 | 30.00 | 23.33 | 26.67 | 13.33 | 30.00 | 33.33 | 33.33 | 24.67 |
| S55 | 43.33 | 23.33 | 30.00 | 20.00 | 26.67 | 43.33 | 36.67 | 30.67 |
| S56 | 23.33 | 40.00 | 23.33 | 30.00 | 30.00 | 33.33 | 36.67 | 20.67 |
| S57 | 23.33 | 26.67 | 30.00 | 23.33 | 26.67 | 26.67 | 33.33 | 28.00 |
| S58 | 16.67 | 23.33 | 26.67 | 26.67 | 23.33 | 20.00 | 13.33 | 19.33 |
| S59 | 16.67 | 30.00 | 30.00 | 30.00 | 30.00 | 16.67 | 30.00 | 24.00 |
| S60 | 20.00 | 33.33 | 20.00 | 26.67 | 20.00 | 43.33 | 30.00 | 28.00 |
| S61 | 13.33 | 26.67 | 16.67 | 20.00 | 26.67 | 13.33 | 13.33 | 17.33 |
| S62 | 30.00 | 33.33 | 36.67 | 30.00 | 33.33 | 30.00 | 40.00 | 31.33 |
| S63 | 26.67 | 23.33 | 26.67 | 23.33 | 20.00 | 30.00 | 30.00 | 28.67 |
| S64 | 26.67 | 23.33 | 26.67 | 23.33 | 23.33 | 33.33 | 26.67 | 23.33 |
| S65 | 26.67 | 23.33 | 30.00 | 20.00 | 26.67 | 26.67 | 23.33 | 26.00 |
| S66 | 33.33 | 36.67 | 43.33 | 50.00 | 43.33 | 23.33 | 30.00 | 35.33 |
| S67 | 23.33 | 23.33 | 26.67 | 30.00 | 26.67 | 30.00 | 30.00 | 28.00 |
| S68 | 20.00 | 16.67 | 26.67 | 16.67 | 30.00 | 23.33 | 16.67 | 20.00 |
| S69 | 23.33 | 23.33 | 26.67 | 23.33 | 20.00 | 23.33 | 23.33 | 23.33 |
| S70 | 30.00 | 30.00 | 26.67 | 30.00 | 26.67 | 23.33 | 33.33 | 31.33 |
| S71 | 36.67 | 20.00 | 40.00 | 20.00 | 26.67 | 46.67 | 30.00 | 34.00 |
| S72 | 33.33 | 50.00 | 33.33 | 43.33 | 60.00 | 56.67 | 40.00 | 44.00 |
| S73 | 33.33 | 23.33 | 20.00 | 23.33 | 23.33 | 33.33 | 23.33 | 24.67 |
| S74 | 26.67 | 23.33 | 16.67 | 23.33 | 26.67 | 23.33 | 23.33 | 22.00 |
| S75 | 36.67 | 30.00 | 26.67 | 40.00 | 30.00 | 23.33 | 30.00 | 31.33 |
| S76 | 33.33 | 30.00 | 33.33 | 26.67 | 33.33 | 36.67 | 30.00 | 27.33 |
| S77 | 26.67 | 23.33 | 26.67 | 23.33 | 23.33 | 23.33 | 20.00 | 24.67 |
| S78 | 20.00 | 26.67 | 30.00 | 26.67 | 33.33 | 23.33 | 26.67 | 22.67 |
| S79 | 20.00 | 16.67 | 36.67 | 33.33 | 20.00 | 20.00 | 20.00 | 27.33 |
| S80 | 30.00 | 20.00 | 33.33 | 40.00 | 23.33 | 30.00 | 33.33 | 32.67 |
| S81 | 36.67 | 26.67 | 33.33 | 30.00 | 30.00 | 26.67 | 30.00 | 30.67 |
| S82 | 26.67 | 20.00 | 33.33 | 23.33 | 26.67 | 26.67 | 23.33 | 25.33 |
| S83 | 26.67 | 23.33 | 16.67 | 20.00 | 20.00 | 33.33 | 30.00 | 22.00 |
| S84 | 33.33 | 23.33 | 46.67 | 26.67 | 53.33 | 40.00 | 30.00 | 26.67 |
| S85 | 46.67 | 43.33 | 23.33 | 40.00 | 40.00 | 53.33 | 36.67 | 50.67 |
| S86 | 23.33 | 23.33 | 36.67 | 23.33 | 23.33 | 16.67 | 23.33 | 24.00 |
| S87 | 26.67 | 30.00 | 20.00 | 23.33 | 26.67 | 30.00 | 16.67 | 27.33 |
| S89 | 23.33 | 23.33 | 30.00 | 23.33 | 23.33 | 33.33 | 26.67 | 32.67 |
| S90 | 10.00 | 23.33 | 10.00 | 33.33 | 30.00 | 23.33 | 23.33 | 22.00 |
| S91 | 36.67 | 43.33 | 33.33 | 40.00 | 30.00 | 30.00 | 23.33 | 38.67 |
| S93 | 43.33 | 23.33 | 30.00 | 26.67 | 36.67 | 36.67 | 23.33 | 32.00 |
| S94 | 23.33 | 33.33 | 20.00 | 10.00 | 23.33 | 26.67 | 30.00 | 18.67 |
| S95 | 16.67 | 23.33 | 10.00 | 23.33 | 20.00 | 20.00 | 20.00 | 20.67 |
| S96 | 26.67 | 30.00 | 40.00 | 30.00 | 33.33 | 26.67 | 30.00 | 26.00 |
| S97 | 16.67 | 20.00 | 26.67 | 23.33 | 20.00 | 20.00 | 30.00 | 24.00 |
| S98 | 16.67 | 20.00 | 40.00 | 23.33 | 23.33 | 20.00 | 26.67 | 31.33 |
| S99 | 0.00 | 10.00 | 16.67 | 20.00 | 16.67 | 10.00 | 10.00 | 6.00 |
| S101 | 23.33 | 26.67 | 46.67 | 23.33 | 23.33 | 26.67 | 26.67 | 25.33 |
| S102 | 20.00 | 26.67 | 30.00 | 30.00 | 30.00 | 23.33 | 30.00 | 28.67 |
| S103 | 30.00 | 40.00 | 23.33 | 33.33 | 36.67 | 23.33 | 23.33 | 26.00 |
| S105 | 26.67 | 20.00 | 33.33 | 30.00 | 30.00 | 30.00 | 30.00 | 30.00 |
| S106 | 30.00 | 36.67 | 36.67 | 30.00 | 36.67 | 30.00 | 33.33 | 32.67 |
| S107 | 33.33 | 20.00 | 20.00 | 20.00 | 16.67 | 16.67 | 23.33 | 21.33 |
| S108 | 13.33 | 20.00 | 23.33 | 16.67 | 33.33 | 30.00 | 23.33 | 19.33 |
| S109 | 30.00 | 23.33 | 26.67 | 30.00 | 26.67 | 30.00 | 20.00 | 28.00 |
| Mean | 27.68 | 27.94 | 27.40 | 28.13 | 28.83 | 28.29 | 28.16 | 28.14 |
| SD | 8.81 | 9.27 | 7.95 | 8.89 | 9.54 | 8.74 | 7.31 | 7.21 |

### T2. Montages and profiles

Full list per subject in `T2_montages.csv` (all 12-channel montages are leave-one-subject-out).

| Method | Distinct montages across subjects | Most frequent montage |
|---|---|---|
| Ours | 98 | F8 AF8 FT7 CP6 T10 T8 O2 C6 PO8 TP8 C4 FT8 |
| CSP | 15 | Fp1 AF7 Fpz Fp2 AF3 AF8 AF4 F5 F7 F8 FC6 AFz |
| RLF | 82 | T8 T10 F7 AF7 FT8 C6 T7 FT7 F8 AF8 TP8 Iz |
| MI | 67 | T8 F8 FC5 AF8 F7 FT8 AF4 C6 T10 F6 C4 AF7 |
| Fixed sensorimotor | 1 | FC3 FC1 FC2 FC4 C3 C1 Cz C2 C4 CP3 CPz CP4 |
| ERD-only | 8 | PO8 O2 O1 PO4 Oz POz PO7 PO3 Fpz P4 P2 Fp2 |

### T3. Equivalence of each 12-channel montage with all 64 channels (paired TOST)

Difference = montage − 64ch, in percentage points. Equivalent means the 90% CI lies inside the margin; it does not mean identical accuracy.

| Method | n | Mean diff (pp) | SD | 90% CI | TOST p | Equivalent (±6 pp) | Worst subject (pp) | Subjects losing >6 pp | Equivalent at margins (pp) |
|---|---|---|---|---|---|---|---|---|---|
| Ours | 105 | +0.25 | 9.13 | [-1.22, +1.73] | <0.0001 | yes | -20.00 | 28 | 2,3,4,5,6,8,10 |
| CSP | 105 | -0.29 | 10.03 | [-1.91, +1.34] | <0.0001 | yes | -36.67 | 28 | 2,3,4,5,6,8,10 |
| RLF | 105 | +0.44 | 9.87 | [-1.15, +2.04] | <0.0001 | yes | -26.67 | 26 | 3,4,5,6,8,10 |
| MI | 105 | +1.14 | 9.15 | [-0.34, +2.62] | <0.0001 | yes | -20.00 | 25 | 3,4,5,6,8,10 |
| Fixed sensorimotor | 105 | +0.60 | 8.06 | [-0.70, +1.91] | <0.0001 | yes | -26.67 | 22 | 2,3,4,5,6,8,10 |
| ERD-only | 105 | +0.48 | 7.80 | [-0.79, +1.74] | <0.0001 | yes | -23.33 | 22 | 2,3,4,5,6,8,10 |
| Random (mean of draws) | 105 | +0.46 | 5.79 | [-0.48, +1.39] | <0.0001 | yes | -15.33 | 11 | 2,3,4,5,6,8,10 |

### T4. Saliency montage (Ours) vs every other 12-channel montage

Positive = Ours more accurate. Holm correction across the comparisons in this table.

| Ours vs | n | Mean diff (pp) | 95% CI | paired t p | Holm | Wilcoxon p | Holm | Ours better / tie / worse |
|---|---|---|---|---|---|---|---|---|
| CSP | 105 | +0.54 | [-1.48, +2.56] | 0.5975 | 1.0000 | 0.6527 | 1.0000 | 45 / 13 / 47 |
| RLF | 105 | -0.19 | [-1.66, +1.28] | 0.7973 | 1.0000 | 0.8615 | 1.0000 | 38 / 28 / 39 |
| MI | 105 | -0.89 | [-2.37, +0.59] | 0.2360 | 1.0000 | 0.2407 | 1.0000 | 34 / 23 / 48 |
| Fixed sensorimotor | 105 | -0.35 | [-2.26, +1.57] | 0.7183 | 1.0000 | 0.4216 | 1.0000 | 41 / 21 / 43 |
| ERD-only | 105 | -0.22 | [-1.84, +1.39] | 0.7856 | 1.0000 | 0.7151 | 1.0000 | 38 / 23 / 44 |
| Random (mean of draws) | 105 | -0.20 | [-1.64, +1.24] | 0.7801 | 1.0000 | 0.5895 | 1.0000 | 46 / 2 / 57 |

### T5. Confusion, class balance and majority baseline (chance 25.0%)

Pooled over all subjects, folds and seeds; full matrices in `T5_confusion_matrices.csv`. The last column flags models that collapsed to one class.

| Method | Pooled acc | Per-class recall | Predicted share per class | Mean majority-class acc | Folds predicting one class ≥90% |
|---|---|---|---|---|---|
| 64ch | 27.68 | left_hand 34.2, right_hand 27.6, hands 22.2, feet 26.7 | left_hand 31.3, right_hand 25.9, hands 19.7, feet 23.1 | 26.67 | 19 / 105 |
| Ours | 27.94 | left_hand 31.1, right_hand 24.9, hands 24.2, feet 31.4 | left_hand 28.0, right_hand 24.6, hands 22.0, feet 25.4 | 26.67 | 25 / 105 |
| CSP | 27.40 | left_hand 24.5, right_hand 27.4, hands 20.8, feet 37.0 | left_hand 22.8, right_hand 27.2, hands 17.7, feet 32.2 | 26.67 | 17 / 105 |
| RLF | 28.13 | left_hand 25.6, right_hand 28.1, hands 23.6, feet 35.2 | left_hand 23.8, right_hand 26.4, hands 20.5, feet 29.2 | 26.67 | 23 / 105 |
| MI | 28.83 | left_hand 27.5, right_hand 29.0, hands 23.5, feet 35.3 | left_hand 23.9, right_hand 27.6, hands 18.8, feet 29.7 | 26.67 | 17 / 105 |
| Fixed sensorimotor | 28.29 | left_hand 36.1, right_hand 29.0, hands 24.6, feet 23.4 | left_hand 31.7, right_hand 26.4, hands 22.3, feet 19.5 | 26.67 | 16 / 105 |
| ERD-only | 28.16 | left_hand 31.3, right_hand 26.7, hands 24.7, feet 29.9 | left_hand 27.8, right_hand 25.6, hands 22.3, feet 24.3 | 26.67 | 18 / 105 |
| Random (mean of draws) | 28.14 | left_hand 31.5, right_hand 27.8, hands 22.7, feet 30.5 | left_hand 27.9, right_hand 26.5, hands 19.9, feet 25.7 | 26.67 | 91 / 525 |

### T6. Seed stability

Grand mean of each single seed, before the seed ensemble used in T1.

| Method | Seeds | Grand mean per seed (%) | Mean across seeds | SD across seeds |
|---|---|---|---|---|
| 64ch | 3 | 42: 26.16, 43: 28.70, 44: 27.21 | 27.35 | 1.28 |
| Ours | 3 | 42: 28.25, 43: 27.46, 44: 27.87 | 27.86 | 0.40 |
| CSP | 3 | 42: 26.57, 43: 27.24, 44: 27.33 | 27.05 | 0.42 |
| RLF | 3 | 42: 27.59, 43: 27.21, 44: 28.63 | 27.81 | 0.74 |
| MI | 3 | 42: 28.32, 43: 28.44, 44: 28.48 | 28.41 | 0.08 |
| Fixed sensorimotor | 3 | 42: 27.62, 43: 28.06, 44: 27.33 | 27.67 | 0.37 |
| ERD-only | 3 | 42: 27.78, 43: 28.25, 44: 27.94 | 27.99 | 0.24 |
| Random (mean of draws) | 3 | 42: 27.73, 43: 28.18, 44: 27.51 | 27.81 | 0.34 |

### T7. Saliency vs ERD/ERS alignment (participant level)

magnitude / class_specific / lateralisation compare unsigned saliency with desynchronisation strength (−ERD) and are sign-invariant; `legacy_signed_LR` is the old statistic, shown only for comparison (its sign is not interpretable). Mean and CI via Fisher z. Per-subject values: `results/full64/alignment_metrics.json`.

| Attribution | Metric | Mean r (Fisher) | 95% CI | SD of r | n subjects |
|---|---|---|---|---|---|
| grad | magnitude_pearson | 0.008 | [-0.044, 0.060] | 0.255 | 105 |
| grad | class_specific_pearson | -0.041 | [-0.087, 0.006] | 0.228 | 105 |
| grad | lateralisation_pearson | -0.054 | [-0.097, -0.011] | 0.213 | 105 |
| grad | magnitude_spearman | -0.028 | [-0.077, 0.022] | 0.244 | 105 |
| grad | class_specific_spearman | -0.028 | [-0.071, 0.015] | 0.213 | 105 |
| grad | lateralisation_spearman | -0.061 | [-0.101, -0.021] | 0.202 | 105 |
| grad | legacy_signed_LR_pearson | -0.007 | [-0.060, 0.045] | 0.259 | 105 |
| grad_x_input | magnitude_pearson | -0.012 | [-0.068, 0.044] | 0.270 | 105 |
| grad_x_input | class_specific_pearson | -0.064 | [-0.115, -0.013] | 0.246 | 105 |
| grad_x_input | lateralisation_pearson | -0.183 | [-0.257, -0.106] | 0.348 | 105 |
| grad_x_input | magnitude_spearman | -0.044 | [-0.095, 0.008] | 0.252 | 105 |
| grad_x_input | class_specific_spearman | -0.057 | [-0.103, -0.010] | 0.229 | 105 |
| grad_x_input | lateralisation_spearman | -0.174 | [-0.247, -0.099] | 0.342 | 105 |
| grad_x_input | legacy_signed_LR_pearson | -0.008 | [-0.067, 0.052] | 0.287 | 105 |
| integrated_gradients | magnitude_pearson | -0.009 | [-0.064, 0.047] | 0.269 | 105 |
| integrated_gradients | class_specific_pearson | -0.063 | [-0.112, -0.013] | 0.241 | 105 |
| integrated_gradients | lateralisation_pearson | -0.186 | [-0.259, -0.110] | 0.344 | 105 |
| integrated_gradients | magnitude_spearman | -0.042 | [-0.094, 0.009] | 0.250 | 105 |
| integrated_gradients | class_specific_spearman | -0.055 | [-0.101, -0.009] | 0.224 | 105 |
| integrated_gradients | lateralisation_spearman | -0.172 | [-0.245, -0.097] | 0.343 | 105 |
| integrated_gradients | legacy_signed_LR_pearson | -0.012 | [-0.071, 0.047] | 0.283 | 105 |
| smoothgrad | magnitude_pearson | 0.008 | [-0.044, 0.060] | 0.256 | 105 |
| smoothgrad | class_specific_pearson | -0.041 | [-0.088, 0.006] | 0.229 | 105 |
| smoothgrad | lateralisation_pearson | -0.059 | [-0.103, -0.016] | 0.215 | 105 |
| smoothgrad | magnitude_spearman | -0.029 | [-0.078, 0.021] | 0.244 | 105 |
| smoothgrad | class_specific_spearman | -0.029 | [-0.071, 0.014] | 0.213 | 105 |
| smoothgrad | lateralisation_spearman | -0.069 | [-0.110, -0.028] | 0.203 | 105 |
| smoothgrad | legacy_signed_LR_pearson | -0.007 | [-0.060, 0.046] | 0.259 | 105 |

### T7b. Correlations as computed by the original scripts

corr(saliency, ERD_L / ERD_R / ERD_(L−R) / ERD_comb) and corr(saliency, plain-gradient saliency), participant level. Kept so the earlier numbers can be compared; an unsigned map is correlated with a signed one, so the sign is not 'agreement' (use T7).

| Attribution | Correlation | Mean r (Fisher) | 95% CI | n subjects |
|---|---|---|---|---|
| grad | ERD_L_pearson | 0.023 | [-0.037, 0.082] | 105 |
| grad | ERD_L_spearman | 0.006 | [-0.051, 0.063] | 105 |
| grad | ERD_R_pearson | 0.050 | [-0.007, 0.107] | 105 |
| grad | ERD_R_spearman | 0.043 | [-0.011, 0.097] | 105 |
| grad | ERD_LR_pearson | -0.007 | [-0.060, 0.045] | 105 |
| grad | ERD_LR_spearman | -0.018 | [-0.070, 0.035] | 105 |
| grad | ERD_comb_pearson | 0.042 | [-0.016, 0.100] | 105 |
| grad | ERD_comb_spearman | 0.023 | [-0.032, 0.077] | 105 |
| grad | vs_grad_pearson | 1.000 | [1.000, 1.000] | 105 |
| grad | vs_grad_spearman | 1.000 | [1.000, 1.000] | 105 |
| grad_x_input | ERD_L_pearson | 0.010 | [-0.056, 0.077] | 105 |
| grad_x_input | ERD_L_spearman | 0.008 | [-0.056, 0.072] | 105 |
| grad_x_input | ERD_R_pearson | 0.035 | [-0.029, 0.098] | 105 |
| grad_x_input | ERD_R_spearman | 0.035 | [-0.023, 0.094] | 105 |
| grad_x_input | ERD_LR_pearson | -0.008 | [-0.067, 0.052] | 105 |
| grad_x_input | ERD_LR_spearman | -0.009 | [-0.067, 0.050] | 105 |
| grad_x_input | ERD_comb_pearson | 0.018 | [-0.047, 0.082] | 105 |
| grad_x_input | ERD_comb_spearman | 0.021 | [-0.040, 0.082] | 105 |
| grad_x_input | vs_grad_pearson | 0.903 | [0.879, 0.922] | 105 |
| grad_x_input | vs_grad_spearman | 0.884 | [0.862, 0.903] | 105 |
| integrated_gradients | ERD_L_pearson | 0.007 | [-0.060, 0.075] | 105 |
| integrated_gradients | ERD_L_spearman | 0.005 | [-0.059, 0.069] | 105 |
| integrated_gradients | ERD_R_pearson | 0.038 | [-0.025, 0.100] | 105 |
| integrated_gradients | ERD_R_spearman | 0.039 | [-0.019, 0.096] | 105 |
| integrated_gradients | ERD_LR_pearson | -0.012 | [-0.071, 0.047] | 105 |
| integrated_gradients | ERD_LR_spearman | -0.015 | [-0.072, 0.043] | 105 |
| integrated_gradients | ERD_comb_pearson | 0.019 | [-0.045, 0.084] | 105 |
| integrated_gradients | ERD_comb_spearman | 0.023 | [-0.038, 0.084] | 105 |
| integrated_gradients | vs_grad_pearson | 0.907 | [0.884, 0.926] | 105 |
| integrated_gradients | vs_grad_spearman | 0.888 | [0.867, 0.906] | 105 |
| smoothgrad | ERD_L_pearson | 0.023 | [-0.036, 0.082] | 105 |
| smoothgrad | ERD_L_spearman | 0.006 | [-0.051, 0.063] | 105 |
| smoothgrad | ERD_R_pearson | 0.050 | [-0.007, 0.107] | 105 |
| smoothgrad | ERD_R_spearman | 0.042 | [-0.012, 0.096] | 105 |
| smoothgrad | ERD_LR_pearson | -0.007 | [-0.060, 0.046] | 105 |
| smoothgrad | ERD_LR_spearman | -0.017 | [-0.070, 0.035] | 105 |
| smoothgrad | ERD_comb_pearson | 0.042 | [-0.016, 0.100] | 105 |
| smoothgrad | ERD_comb_spearman | 0.023 | [-0.032, 0.077] | 105 |
| smoothgrad | vs_grad_pearson | 1.000 | [1.000, 1.000] | 105 |
| smoothgrad | vs_grad_spearman | 0.999 | [0.999, 0.999] | 105 |

### T10. EXPLORATORY: saliency vs other physiological maps

Curiosity only — not used for any choice; the paper's alignment is T7. Saliency = mean of the four attribution maps (`mean4`); per method in `T10_physiology_all_methods.csv`. r = corr(saliency, map), |map| = corr(saliency, |map|), class-specific = mean of corr(saliency_L, |map_L|) and corr(saliency_R, |map_R|). Fisher-z mean over subjects. Group maps: `figures/physiology_maps_group.png`.

| Map | Pearson r | 95% CI | Pearson r (|map|) | Spearman r | Spearman r (|map|) | n |
|---|---|---|---|---|---|---|
| ERD_theta_L | -0.062 | [-0.130, 0.006] | -0.030 | -0.049 | -0.035 | 105 |
| ERD_theta_R | -0.030 | [-0.093, 0.032] | 0.007 | -0.031 | 0.003 | 105 |
| ERD_theta_mag | -0.025 | [-0.087, 0.038] | -0.025 | -0.027 | -0.027 | 105 |
| ERD_mu_L | 0.017 | [-0.042, 0.075] | 0.038 | 0.003 | 0.020 | 105 |
| ERD_mu_R | 0.050 | [-0.010, 0.110] | -0.019 | 0.051 | -0.043 | 105 |
| ERD_mu_mag | 0.011 | [-0.045, 0.067] | 0.011 | -0.024 | -0.024 | 105 |
| ERD_beta_L | 0.021 | [-0.043, 0.085] | -0.001 | 0.016 | -0.020 | 105 |
| ERD_beta_R | 0.022 | [-0.036, 0.081] | -0.007 | 0.014 | -0.019 | 105 |
| ERD_beta_mag | -0.006 | [-0.051, 0.039] | -0.006 | -0.024 | -0.024 | 105 |
| ERS_beta_rebound_L | 0.008 | [-0.056, 0.073] | 0.025 | -0.000 | 0.009 | 105 |
| ERS_beta_rebound_R | 0.009 | [-0.053, 0.071] | -0.015 | -0.000 | -0.036 | 105 |
| ERS_beta_rebound_mag | 0.002 | [-0.055, 0.060] | 0.002 | -0.019 | -0.019 | 105 |
| ERD_lowgamma_L | 0.007 | [-0.042, 0.056] | -0.031 | -0.003 | -0.041 | 105 |
| ERD_lowgamma_R | -0.002 | [-0.060, 0.056] | 0.026 | -0.005 | 0.015 | 105 |
| ERD_lowgamma_mag | -0.002 | [-0.052, 0.048] | -0.002 | -0.018 | -0.018 | 105 |
| logpow_8_30 | 0.044 | [-0.012, 0.101] | 0.044 | 0.033 | 0.033 | 105 |
| r2_signed | 0.053 | [-0.001, 0.106] | -0.017 | 0.042 | -0.021 | 105 |
| r2_abs | -0.017 | [-0.070, 0.037] | -0.017 | -0.021 | -0.021 | 105 |
| TFR_ERD_dB_L | -0.004 | [-0.065, 0.058] | 0.022 | -0.009 | 0.002 | 105 |
| TFR_ERD_dB_R | 0.019 | [-0.037, 0.075] | -0.027 | 0.019 | -0.033 | 105 |
| TFR_ERD_dB_mag | -0.002 | [-0.048, 0.045] | -0.002 | -0.021 | -0.021 | 105 |
| ITC_4_30 | -0.030 | [-0.085, 0.025] | -0.030 | -0.038 | -0.038 | 105 |
| ERP_abs_0.2_0.8 | -0.069 | [-0.126, -0.011] | -0.069 | -0.093 | -0.093 | 105 |
| SlowPot_0.5_3 | -0.002 | [-0.061, 0.057] | 0.014 | 0.000 | 0.004 | 105 |
| ERD_beta_classspecific | — | — | 0.003 [-0.030, 0.035] | — | -0.013 | 105 |
| ERD_lowgamma_classspecific | — | — | -0.002 [-0.040, 0.036] | — | -0.010 | 105 |
| ERD_mu_classspecific | — | — | 0.005 [-0.036, 0.046] | — | -0.012 | 105 |
| ERD_theta_classspecific | — | — | -0.013 [-0.064, 0.037] | — | -0.012 | 105 |
| ERS_beta_rebound_classspecific | — | — | 0.003 [-0.038, 0.044] | — | -0.011 | 105 |
| TFR_ERD_dB_classspecific | — | — | -0.005 [-0.040, 0.029] | — | -0.016 | 105 |

### T8a. Faithfulness: deletion test on the test trials

Accuracy drop (intact − channels removed), mean ± SD across subjects. Ranking from validation saliency; removal = channel set to its standardised mean. A faithful ranking gives the largest drop for top-ranked channels.

| Removed channels k | Drop: top-ranked (pp) | Drop: random (pp) | Drop: bottom-ranked (pp) | top vs random p | top vs bottom p |
|---|---|---|---|---|---|
| 2 | +0.70 ± 2.42 | +0.16 ± 1.26 | +0.05 ± 1.42 | 0.0050 | 0.0061 |
| 4 | +0.90 ± 3.15 | +0.41 ± 1.95 | +0.22 ± 1.78 | 0.0140 | 0.0133 |
| 6 | +1.17 ± 4.12 | +0.60 ± 2.54 | +0.37 ± 2.21 | 0.0298 | 0.0182 |

### T8b. Model-randomisation sanity check

Similarity between saliency of the trained model and of an untrained model. High values mean the map reflects the input more than what the network learned.

| Attribution | Spearman(trained, untrained model) | 95% CI | n subjects |
|---|---|---|---|
| grad | -0.004 | [-0.018, 0.009] | 105 |
| grad_x_input | 0.207 | [0.166, 0.248] | 105 |
| integrated_gradients | 0.198 | [0.156, 0.239] | 105 |
| smoothgrad | -0.005 | [-0.019, 0.008] | 105 |

### T9. Configuration

Full snapshot: `T9_config.json`.

Training profile chosen on validation data only, leave-one-subject-out (unanimous: True): S01=zscore, S02=zscore, S03=zscore, S04=zscore, S05=zscore, S06=zscore, S07=zscore, S08=zscore, S09=zscore, S10=zscore, S11=zscore, S12=zscore, S13=zscore, S14=zscore, S15=zscore, S16=zscore, S17=zscore, S18=zscore, S19=zscore, S20=zscore, S21=zscore, S22=zscore, S23=zscore, S24=zscore, S25=zscore, S26=zscore, S27=zscore, S28=zscore, S29=zscore, S30=zscore, S31=zscore, S32=zscore, S33=zscore, S34=zscore, S35=zscore, S36=zscore, S37=zscore, S38=zscore, S39=zscore, S40=zscore, S41=zscore, S42=zscore, S43=zscore, S44=zscore, S45=zscore, S46=zscore, S47=zscore, S48=zscore, S49=zscore, S50=zscore, S51=zscore, S52=zscore, S53=zscore, S54=zscore, S55=zscore, S56=zscore, S57=zscore, S58=zscore, S59=zscore, S60=zscore, S61=zscore, S62=zscore, S63=zscore, S64=zscore, S65=zscore, S66=zscore, S67=zscore, S68=zscore, S69=zscore, S70=zscore, S71=zscore, S72=zscore, S73=zscore, S74=zscore, S75=zscore, S76=zscore, S77=zscore, S78=zscore, S79=zscore, S80=zscore, S81=zscore, S82=zscore, S83=zscore, S84=zscore, S85=zscore, S86=zscore, S87=zscore, S89=zscore, S90=zscore, S91=zscore, S93=zscore, S94=zscore, S95=zscore, S96=zscore, S97=zscore, S98=zscore, S99=zscore, S101=zscore, S102=zscore, S103=zscore, S105=zscore, S106=zscore, S107=zscore, S108=zscore, S109=zscore

| Profile | Mean validation accuracy (%) |
|---|---|
| zscore | 40.48 |
| ems | 38.75 |
| original | 29.46 |

```
model: "Deep4Net"
dataset: "PhysionetMI"
sfreq_hz: "per profile (profiles[*].sfreq)"
profiles: {"zscore": {"sfreq": 160, "band_hz": [4.0, 40.0], "window_s": [0.0, 3.0], "car": false, "norm": null, "align": "zscore", "dropout": 0.5, "pool_time_length": 3, "pool_time_stride": 3, "lr": 0.001, "weight_decay": 0.0005, "scheduler": "cosine", "max_epochs": 300, "patience": 80, "batch_size": 16, "label_smoothing": 0.1, "grad_clip": 10.0, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "ems": {"sfreq": 160, "band_hz": [4.0, 40.0], "window_s": [0.0, 3.0], "car": false, "norm": "ems", "align": null, "dropout": 0.5, "pool_time_length": 3, "pool_time_stride": 3, "lr": 0.001, "weight_decay": 0.0005, "scheduler": "cosine", "max_epochs": 300, "patience": 80, "batch_size": 16, "label_smoothing": 0.1, "grad_clip": 10.0, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "original": {"sfreq": 160, "band_hz": [8.0, 32.0], "window_s": [0.5, 2.5], "norm": null, "align": null, "car": false, "dropout": 0.25, "pool_time_length": 2, "pool_time_stride": 2, "lr": 0.01, "weight_decay": 1e-05, "scheduler": "multistep", "milestones": [20, 50], "gamma": 0.1, "max_epochs": 100, "patience": 100, "batch_size": 64, "label_smoothing": 0.0, "grad_clip": 10.0, "augment": false, "select_on": "val_loss", "min_select_epoch": 1}}
checkpoint_rule: "highest validation accuracy (loss breaks ties), not before epoch 20 ('original': lowest validation loss); refit keeps the final weights"
folds: "run-wise chronological split per subject: test = the last imagery run of each type (run 12 left/right, run 14 hands/feet); training = runs 4, 8 (and 6, 10); validation = the chronologically last 25% of the training trials of EACH class; refit on all training runs"
seeds: [42, 43, 44]
```

Figures (530 topomaps: saliency per method/subject, group maps, ERD/ERS) copied to `4class\figures`.
