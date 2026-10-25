# Results report — EEGItNet\HGD

Generated 2026-10-22 13:02 from the saved `results.json` files. TOST margin ±6 percentage points. Results folder: `<class>/results_session/`.

## 2class

### T1. Test accuracy (%) per subject — chance 50.0%

Protocol: train on the official HGD training runs (last 25% = validation, chronological), refit on all training runs, test once on the official test runs. Subject accuracy = seed ensemble (mean softmax of 3 seeds); single seeds in T6. SD = across subjects (n = 14). Random = mean of the random-montage draws.

| Method | S01 | S02 | S03 | S04 | S05 | S06 | S07 | S08 | S09 | S10 | S11 | S12 | S13 | S14 | Mean | SD |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 22ch | 53.75 | 76.25 | 95.00 | 100.00 | 61.25 | 72.50 | 50.00 | 56.25 | 50.00 | 97.50 | 62.50 | 96.25 | 78.75 | 93.75 | 74.55 | 19.12 |
| Ours | 50.00 | 56.25 | 96.25 | 96.25 | 63.75 | 63.75 | 50.00 | 56.25 | 52.50 | 97.50 | 63.75 | 90.00 | 75.00 | 92.50 | 71.70 | 18.87 |
| CSP | 51.25 | 52.50 | 95.00 | 100.00 | 52.50 | 76.25 | 56.25 | 52.50 | 50.00 | 100.00 | 57.50 | 95.00 | 73.75 | 93.75 | 71.88 | 20.82 |
| RLF | 52.50 | 83.75 | 93.75 | 91.25 | 52.50 | 87.50 | 58.75 | 52.50 | 58.75 | 98.75 | 55.00 | 96.25 | 75.00 | 97.50 | 75.27 | 19.25 |
| MI | 53.75 | 51.25 | 97.50 | 95.00 | 63.75 | 81.25 | 53.75 | 50.00 | 51.25 | 96.25 | 63.75 | 97.50 | 58.75 | 90.00 | 71.70 | 19.90 |
| Fixed sensorimotor | 56.25 | 80.00 | 93.75 | 97.50 | 62.50 | 72.50 | 62.50 | 56.25 | 53.75 | 98.75 | 62.50 | 97.50 | 70.00 | 95.00 | 75.62 | 17.55 |
| ERD-only | 61.25 | 75.00 | 98.75 | 96.25 | 71.25 | 78.75 | 55.00 | 47.50 | 50.00 | 100.00 | 67.50 | 97.50 | 77.50 | 95.00 | 76.52 | 18.76 |
| Random (mean of draws) | 55.25 | 66.00 | 97.25 | 92.75 | 61.25 | 71.00 | 57.00 | 56.00 | 52.50 | 99.00 | 63.25 | 96.75 | 72.00 | 90.00 | 73.57 | 17.69 |

### T0. Data used per subject

Trials after the class selection of this experiment (training trials include the validation part, which is also used to fit the final model; the test trials are never used for any choice).

| Subject | Training trials (incl. validation) | Validation trials | Test trials | Test trials per class | Majority-class test accuracy (%) | Chance (%) |
|---|---|---|---|---|---|---|
| S01 | 160 | 40 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S02 | 406 | 102 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S03 | 440 | 110 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S04 | 448 | 112 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S05 | 360 | 90 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S06 | 440 | 110 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S07 | 440 | 110 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S08 | 328 | 82 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S09 | 440 | 110 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S10 | 440 | 110 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S11 | 440 | 110 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S12 | 440 | 110 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S13 | 400 | 100 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |
| S14 | 440 | 110 | 80 | left_hand 40, right_hand 40 | 50.00 | 50.00 |

### T2. Montages and profiles

Full list per subject in `T2_montages.csv` (all 12-channel montages are leave-one-subject-out).

| Method | Distinct montages across subjects | Most frequent montage |
|---|---|---|
| Ours | 14 | CP3 CP6 CP5 C6 FC6 C3 FC5 Pz C5 C4 CP1 CP2 |
| CSP | 13 | CP6 CP5 FC5 C6 C5 Pz FC6 CP3 C4 C3 FC4 FC3 |
| RLF | 14 | CP2 CP3 CP1 CP4 C4 C2 C1 FC2 CP6 C3 FC1 FCz |
| MI | 14 | C6 C2 CP4 C4 C3 CP6 CP2 FC5 FC3 CP1 FC4 C5 |
| Fixed sensorimotor | 1 | FC3 FC1 FC2 FC4 C3 C1 Cz C2 C4 CP3 CPz CP4 |
| ERD-only | 13 | C4 C2 C1 C3 CP3 CP1 CP2 Pz CP6 CP4 CP5 CPz |

### T3. Equivalence of each 12-channel montage with all 22 channels (paired TOST)

Difference = montage − 22ch, in percentage points. Equivalent means the 90% CI lies inside the margin; it does not mean identical accuracy.

| Method | n | Mean diff (pp) | SD | 90% CI | TOST p | Equivalent (±6 pp) | Worst subject (pp) | Subjects losing >6 pp | Equivalent at margins (pp) |
|---|---|---|---|---|---|---|---|---|---|
| Ours | 14 | -2.86 | 5.95 | [-5.67, -0.04] | 0.0349 | yes | -20.00 | 3 | 6,8,10 |
| CSP | 14 | -2.68 | 7.19 | [-6.08, +0.72] | 0.0537 | no | -23.75 | 2 | 8,10 |
| RLF | 14 | +0.71 | 7.25 | [-2.72, +4.15] | 0.0086 | yes | -8.75 | 3 | 5,6,8,10 |
| MI | 14 | -2.86 | 9.19 | [-7.21, +1.49] | 0.1116 | no | -25.00 | 3 | 8,10 |
| Fixed sensorimotor | 14 | +1.07 | 4.52 | [-1.07, +3.21] | 0.0006 | yes | -8.75 | 1 | 4,5,6,8,10 |
| ERD-only | 14 | +1.96 | 4.87 | [-0.34, +4.27] | 0.0042 | yes | -8.75 | 1 | 5,6,8,10 |
| Random (mean of draws) | 14 | -0.98 | 4.57 | [-3.15, +1.18] | 0.0006 | yes | -10.25 | 3 | 4,5,6,8,10 |

### T4. Saliency montage (Ours) vs every other 12-channel montage

Positive = Ours more accurate. Holm correction across the comparisons in this table.

| Ours vs | n | Mean diff (pp) | 95% CI | paired t p | Holm | Wilcoxon p | Holm | Ours better / tie / worse |
|---|---|---|---|---|---|---|---|---|
| CSP | 14 | -0.18 | [-3.56, +3.20] | 0.9110 | 1.0000 | 0.9749 | 1.0000 | 7 / 0 / 7 |
| RLF | 14 | -3.57 | [-9.93, +2.79] | 0.2467 | 0.7401 | 0.3633 | 1.0000 | 5 / 1 / 8 |
| MI | 14 | +0.00 | [-4.33, +4.33] | 1.0000 | 1.0000 | 0.8443 | 1.0000 | 7 / 2 / 5 |
| Fixed sensorimotor | 14 | -3.93 | [-8.23, +0.37] | 0.0701 | 0.3506 | 0.0738 | 0.3692 | 4 / 1 / 9 |
| ERD-only | 14 | -4.82 | [-8.86, -0.78] | 0.0230 | 0.1379 | 0.0249 | 0.1493 | 2 / 1 / 11 |
| Random (mean of draws) | 14 | -1.87 | [-4.45, +0.70] | 0.1392 | 0.5568 | 0.2489 | 0.9955 | 6 / 1 / 7 |

### T5. Confusion, class balance and majority baseline (chance 50.0%)

Pooled over all subjects, folds and seeds; full matrices in `T5_confusion_matrices.csv`, per subject in `T5_confusion_per_subject.csv`. The last column flags models that collapsed to one class.

| Method | Pooled acc | Per-class recall | Predicted share per class | Mean majority-class acc | Folds predicting one class ≥90% |
|---|---|---|---|---|---|
| 22ch | 74.55 | left_hand 70.2, right_hand 78.9 | left_hand 45.6, right_hand 54.4 | 50.00 | 1 / 14 |
| Ours | 71.70 | left_hand 72.3, right_hand 71.1 | left_hand 50.6, right_hand 49.4 | 50.00 | 1 / 14 |
| CSP | 71.88 | left_hand 69.6, right_hand 74.1 | left_hand 47.8, right_hand 52.2 | 50.00 | 2 / 14 |
| RLF | 75.27 | left_hand 72.9, right_hand 77.7 | left_hand 47.6, right_hand 52.4 | 50.00 | 1 / 14 |
| MI | 71.70 | left_hand 71.4, right_hand 72.0 | left_hand 49.7, right_hand 50.3 | 50.00 | 2 / 14 |
| Fixed sensorimotor | 75.62 | left_hand 71.8, right_hand 79.5 | left_hand 46.2, right_hand 53.8 | 50.00 | 1 / 14 |
| ERD-only | 76.52 | left_hand 75.5, right_hand 77.5 | left_hand 49.0, right_hand 51.0 | 50.00 | 1 / 14 |
| Random (mean of draws) | 73.57 | left_hand 70.6, right_hand 76.6 | left_hand 47.0, right_hand 53.0 | 50.00 | 4 / 70 |

### T6. Seed stability

Grand mean of each single seed, before the seed ensemble used in T1.

| Method | Seeds | Grand mean per seed (%) | Mean across seeds | SD across seeds |
|---|---|---|---|---|
| 22ch | 3 | 42: 74.73, 43: 69.55, 44: 74.46 | 72.92 | 2.92 |
| Ours | 3 | 42: 71.52, 43: 69.29, 44: 70.80 | 70.54 | 1.14 |
| CSP | 3 | 42: 70.18, 43: 68.66, 44: 70.36 | 69.73 | 0.93 |
| RLF | 3 | 42: 70.00, 43: 71.70, 44: 73.57 | 71.76 | 1.79 |
| MI | 3 | 42: 67.86, 43: 66.79, 44: 70.00 | 68.21 | 1.64 |
| Fixed sensorimotor | 3 | 42: 72.95, 43: 71.52, 44: 74.55 | 73.01 | 1.52 |
| ERD-only | 3 | 42: 73.57, 43: 70.62, 44: 74.73 | 72.98 | 2.12 |
| Random (mean of draws) | 3 | 42: 69.64, 43: 70.32, 44: 71.21 | 70.39 | 0.79 |

### T7. Saliency vs ERD/ERS alignment (participant level)

magnitude / class_specific / lateralisation compare unsigned saliency with desynchronisation strength (−ERD) and are sign-invariant; `legacy_signed_LR` is the old statistic, shown only for comparison (its sign is not interpretable). Mean and CI via Fisher z. Per-subject values: `results/full22/alignment_metrics.json`.

| Attribution | Metric | Mean r (Fisher) | 95% CI | SD of r | n subjects |
|---|---|---|---|---|---|
| grad | magnitude_pearson | 0.012 | [-0.084, 0.109] | 0.163 | 14 |
| grad | class_specific_pearson | 0.123 | [-0.008, 0.250] | 0.212 | 14 |
| grad | lateralisation_pearson | -0.051 | [-0.209, 0.109] | 0.260 | 14 |
| grad | magnitude_spearman | 0.098 | [0.008, 0.187] | 0.154 | 14 |
| grad | class_specific_spearman | 0.163 | [0.050, 0.272] | 0.188 | 14 |
| grad | lateralisation_spearman | -0.035 | [-0.189, 0.120] | 0.255 | 14 |
| grad | legacy_signed_LR_pearson | 0.077 | [-0.080, 0.230] | 0.253 | 14 |
| grad_x_input | magnitude_pearson | 0.090 | [-0.082, 0.257] | 0.283 | 14 |
| grad_x_input | class_specific_pearson | 0.078 | [-0.071, 0.224] | 0.249 | 14 |
| grad_x_input | lateralisation_pearson | -0.314 | [-0.548, -0.034] | 0.400 | 14 |
| grad_x_input | magnitude_spearman | -0.053 | [-0.312, 0.214] | 0.358 | 14 |
| grad_x_input | class_specific_spearman | -0.017 | [-0.172, 0.139] | 0.259 | 14 |
| grad_x_input | lateralisation_spearman | -0.287 | [-0.516, -0.021] | 0.400 | 14 |
| grad_x_input | legacy_signed_LR_pearson | 0.168 | [0.019, 0.309] | 0.246 | 14 |
| integrated_gradients | magnitude_pearson | 0.081 | [-0.090, 0.247] | 0.279 | 14 |
| integrated_gradients | class_specific_pearson | 0.070 | [-0.079, 0.216] | 0.249 | 14 |
| integrated_gradients | lateralisation_pearson | -0.270 | [-0.505, 0.003] | 0.384 | 14 |
| integrated_gradients | magnitude_spearman | -0.060 | [-0.349, 0.240] | 0.366 | 14 |
| integrated_gradients | class_specific_spearman | -0.024 | [-0.173, 0.125] | 0.249 | 14 |
| integrated_gradients | lateralisation_spearman | -0.252 | [-0.480, 0.007] | 0.386 | 14 |
| integrated_gradients | legacy_signed_LR_pearson | 0.152 | [-0.001, 0.298] | 0.253 | 14 |
| smoothgrad | magnitude_pearson | 0.013 | [-0.084, 0.109] | 0.164 | 14 |
| smoothgrad | class_specific_pearson | 0.125 | [-0.006, 0.251] | 0.212 | 14 |
| smoothgrad | lateralisation_pearson | -0.051 | [-0.208, 0.108] | 0.258 | 14 |
| smoothgrad | magnitude_spearman | 0.099 | [0.009, 0.187] | 0.152 | 14 |
| smoothgrad | class_specific_spearman | 0.165 | [0.049, 0.276] | 0.192 | 14 |
| smoothgrad | lateralisation_spearman | -0.039 | [-0.193, 0.118] | 0.257 | 14 |
| smoothgrad | legacy_signed_LR_pearson | 0.078 | [-0.078, 0.231] | 0.253 | 14 |

### T7b. Correlations as computed by the original scripts

corr(saliency, ERD_L / ERD_R / ERD_(L−R) / ERD_comb) and corr(saliency, plain-gradient saliency), participant level. Kept so the earlier numbers can be compared; an unsigned map is correlated with a signed one, so the sign is not 'agreement' (use T7).

| Attribution | Correlation | Mean r (Fisher) | 95% CI | n subjects |
|---|---|---|---|---|
| grad | ERD_L_pearson | -0.142 | [-0.303, 0.028] | 14 |
| grad | ERD_L_spearman | -0.187 | [-0.327, -0.038] | 14 |
| grad | ERD_R_pearson | -0.111 | [-0.217, -0.002] | 14 |
| grad | ERD_R_spearman | -0.155 | [-0.260, -0.045] | 14 |
| grad | ERD_LR_pearson | 0.077 | [-0.080, 0.230] | 14 |
| grad | ERD_LR_spearman | 0.028 | [-0.121, 0.176] | 14 |
| grad | ERD_comb_pearson | -0.111 | [-0.227, 0.008] | 14 |
| grad | ERD_comb_spearman | -0.153 | [-0.268, -0.034] | 14 |
| grad | vs_grad_pearson | 1.000 | [1.000, 1.000] | 14 |
| grad | vs_grad_spearman | 1.000 | [1.000, 1.000] | 14 |
| grad_x_input | ERD_L_pearson | -0.041 | [-0.198, 0.118] | 14 |
| grad_x_input | ERD_L_spearman | 0.070 | [-0.082, 0.219] | 14 |
| grad_x_input | ERD_R_pearson | -0.124 | [-0.266, 0.024] | 14 |
| grad_x_input | ERD_R_spearman | -0.071 | [-0.306, 0.173] | 14 |
| grad_x_input | ERD_LR_pearson | 0.168 | [0.019, 0.309] | 14 |
| grad_x_input | ERD_LR_spearman | 0.221 | [-0.009, 0.429] | 14 |
| grad_x_input | ERD_comb_pearson | -0.093 | [-0.249, 0.068] | 14 |
| grad_x_input | ERD_comb_spearman | -0.035 | [-0.286, 0.220] | 14 |
| grad_x_input | vs_grad_pearson | 0.291 | [0.153, 0.417] | 14 |
| grad_x_input | vs_grad_spearman | 0.282 | [0.165, 0.390] | 14 |
| integrated_gradients | ERD_L_pearson | -0.036 | [-0.195, 0.124] | 14 |
| integrated_gradients | ERD_L_spearman | 0.074 | [-0.087, 0.230] | 14 |
| integrated_gradients | ERD_R_pearson | -0.120 | [-0.267, 0.033] | 14 |
| integrated_gradients | ERD_R_spearman | -0.081 | [-0.348, 0.198] | 14 |
| integrated_gradients | ERD_LR_pearson | 0.152 | [-0.001, 0.298] | 14 |
| integrated_gradients | ERD_LR_spearman | 0.212 | [-0.044, 0.441] | 14 |
| integrated_gradients | ERD_comb_pearson | -0.091 | [-0.252, 0.075] | 14 |
| integrated_gradients | ERD_comb_spearman | -0.048 | [-0.330, 0.242] | 14 |
| integrated_gradients | vs_grad_pearson | 0.269 | [0.153, 0.377] | 14 |
| integrated_gradients | vs_grad_spearman | 0.281 | [0.170, 0.384] | 14 |
| smoothgrad | ERD_L_pearson | -0.143 | [-0.304, 0.026] | 14 |
| smoothgrad | ERD_L_spearman | -0.187 | [-0.327, -0.038] | 14 |
| smoothgrad | ERD_R_pearson | -0.112 | [-0.218, -0.003] | 14 |
| smoothgrad | ERD_R_spearman | -0.153 | [-0.259, -0.043] | 14 |
| smoothgrad | ERD_LR_pearson | 0.078 | [-0.078, 0.231] | 14 |
| smoothgrad | ERD_LR_spearman | 0.031 | [-0.122, 0.181] | 14 |
| smoothgrad | ERD_comb_pearson | -0.112 | [-0.228, 0.007] | 14 |
| smoothgrad | ERD_comb_spearman | -0.152 | [-0.267, -0.033] | 14 |
| smoothgrad | vs_grad_pearson | 1.000 | [1.000, 1.000] | 14 |
| smoothgrad | vs_grad_spearman | 1.000 | [1.000, 1.000] | 14 |

### T10. EXPLORATORY: saliency vs other physiological maps

Curiosity only — not used for any choice; the paper's alignment is T7. Saliency = mean of the four attribution maps (`mean4`); per method in `T10_physiology_all_methods.csv`. r = corr(saliency, map), |map| = corr(saliency, |map|), class-specific = mean of corr(saliency_L, |map_L|) and corr(saliency_R, |map_R|). Fisher-z mean over subjects. Group maps: `figures/physiology_maps_group.png`.

| Map | Pearson r | 95% CI | Pearson r (|map|) | Spearman r | Spearman r (|map|) | n |
|---|---|---|---|---|---|---|
| ERD_theta_L | -0.025 | [-0.223, 0.175] | 0.178 | -0.012 | 0.189 | 14 |
| ERD_theta_R | -0.117 | [-0.292, 0.064] | -0.024 | -0.120 | 0.023 | 14 |
| ERD_theta_mag | 0.034 | [-0.175, 0.240] | 0.034 | 0.071 | 0.071 | 14 |
| ERD_mu_L | -0.062 | [-0.172, 0.049] | 0.084 | 0.010 | 0.068 | 14 |
| ERD_mu_R | -0.127 | [-0.232, -0.020] | -0.007 | -0.085 | -0.022 | 14 |
| ERD_mu_mag | -0.013 | [-0.158, 0.134] | -0.013 | -0.030 | -0.030 | 14 |
| ERD_beta_L | -0.207 | [-0.322, -0.086] | 0.198 | -0.096 | 0.110 | 14 |
| ERD_beta_R | -0.230 | [-0.336, -0.119] | 0.117 | -0.123 | 0.002 | 14 |
| ERD_beta_mag | 0.119 | [-0.040, 0.272] | 0.119 | 0.017 | 0.017 | 14 |
| ERS_beta_rebound_L | -0.046 | [-0.201, 0.110] | 0.172 | -0.003 | 0.086 | 14 |
| ERS_beta_rebound_R | -0.072 | [-0.241, 0.102] | 0.094 | -0.012 | 0.031 | 14 |
| ERS_beta_rebound_mag | 0.133 | [0.013, 0.250] | 0.133 | 0.041 | 0.041 | 14 |
| ERD_lowgamma_L | -0.126 | [-0.312, 0.069] | 0.214 | -0.051 | 0.128 | 14 |
| ERD_lowgamma_R | -0.162 | [-0.297, -0.021] | 0.106 | -0.079 | 0.046 | 14 |
| ERD_lowgamma_mag | 0.124 | [-0.039, 0.281] | 0.124 | 0.053 | 0.053 | 14 |
| ERD_highgamma_L | -0.092 | [-0.279, 0.102] | 0.278 | -0.053 | 0.312 | 14 |
| ERD_highgamma_R | -0.006 | [-0.166, 0.154] | 0.035 | -0.004 | 0.063 | 14 |
| ERD_highgamma_mag | 0.172 | [-0.036, 0.366] | 0.172 | 0.217 | 0.217 | 14 |
| logpow_8_30 | 0.526 | [0.405, 0.629] | 0.289 | 0.583 | 0.351 | 14 |
| r2_signed | -0.058 | [-0.225, 0.112] | 0.142 | -0.081 | 0.096 | 14 |
| r2_abs | 0.142 | [-0.004, 0.281] | 0.142 | 0.096 | 0.096 | 14 |
| TFR_ERD_dB_L | -0.149 | [-0.268, -0.026] | 0.138 | -0.101 | 0.110 | 14 |
| TFR_ERD_dB_R | -0.198 | [-0.328, -0.061] | 0.048 | -0.128 | 0.010 | 14 |
| TFR_ERD_dB_mag | 0.049 | [-0.125, 0.220] | 0.049 | 0.031 | 0.031 | 14 |
| ITC_4_30 | 0.378 | [0.190, 0.539] | 0.378 | 0.338 | 0.338 | 14 |
| ERP_abs_0.2_0.8 | 0.350 | [0.170, 0.507] | 0.350 | 0.387 | 0.387 | 14 |
| SlowPot_0.5_3 | -0.200 | [-0.383, -0.003] | 0.315 | -0.207 | 0.308 | 14 |
| ERD_beta_classspecific | — | — | 0.156 [0.046, 0.261] | — | 0.062 | 14 |
| ERD_highgamma_classspecific | — | — | 0.155 [0.039, 0.266] | — | 0.187 | 14 |
| ERD_lowgamma_classspecific | — | — | 0.160 [0.053, 0.264] | — | 0.090 | 14 |
| ERD_mu_classspecific | — | — | 0.035 [-0.068, 0.136] | — | 0.022 | 14 |
| ERD_theta_classspecific | — | — | 0.071 [-0.080, 0.219] | — | 0.102 | 14 |
| ERS_beta_rebound_classspecific | — | — | 0.133 [0.027, 0.236] | — | 0.066 | 14 |
| TFR_ERD_dB_classspecific | — | — | 0.094 [-0.011, 0.196] | — | 0.063 | 14 |

### T8a. Faithfulness: deletion test on the test trials

Accuracy drop (intact − channels removed), mean ± SD across subjects. Ranking from validation saliency; removal = channel set to its standardised mean. A faithful ranking gives the largest drop for top-ranked channels.

| Removed channels k | Drop: top-ranked (pp) | Drop: random (pp) | Drop: bottom-ranked (pp) | top vs random p | top vs bottom p |
|---|---|---|---|---|---|
| 2 | +13.21 ± 13.88 | +6.46 ± 6.01 | +1.34 ± 2.84 | 0.0104 | 0.0040 |
| 4 | +15.77 ± 14.55 | +10.82 ± 9.73 | +3.96 ± 6.56 | 0.0064 | 0.0018 |
| 6 | +18.63 ± 18.53 | +13.43 ± 11.97 | +6.52 ± 7.37 | 0.0300 | 0.0166 |

### T8b. Model-randomisation sanity check

Similarity between saliency of the trained model and of an untrained model. High values mean the map reflects the input more than what the network learned.

| Attribution | Spearman(trained, untrained model) | 95% CI | n subjects |
|---|---|---|---|
| grad | 0.075 | [0.015, 0.135] | 14 |
| grad_x_input | 0.689 | [0.622, 0.745] | 14 |
| integrated_gradients | 0.682 | [0.622, 0.734] | 14 |
| smoothgrad | 0.083 | [0.022, 0.144] | 14 |

### T9. Configuration

Full snapshot: `T9_config.json`.

Training profile chosen on validation data only, leave-one-subject-out (unanimous: True): S01=original, S02=original, S03=original, S04=original, S05=original, S06=original, S07=original, S08=original, S09=original, S10=original, S11=original, S12=original, S13=original, S14=original

| Profile | Mean validation accuracy (%) |
|---|---|
| original | 78.27 |
| ems | 76.44 |
| salami128 | 71.84 |

```
model: "EEGITNet"
dataset: "Schirrmeister2017"
sfreq_hz: "per profile (profiles[*].sfreq)"
profiles: {"original": {"sfreq": 100, "band_hz": [4.0, 38.0], "window_s": [0.0, 4.0], "norm": null, "car": false, "lr": 0.0005, "weight_decay": 0.0001, "scheduler": "plateau", "plateau_factor": 0.5, "plateau_patience": 30, "max_epochs": 600, "patience": 150, "batch_size": 96, "label_smoothing": 0.1, "grad_clip": 10.0, "dropout": 0.3, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "ems": {"sfreq": 100, "band_hz": [4.0, 38.0], "window_s": [0.0, 4.0], "norm": "ems", "car": false, "lr": 0.0005, "weight_decay": 0.0001, "scheduler": "plateau", "plateau_factor": 0.5, "plateau_patience": 30, "max_epochs": 600, "patience": 150, "batch_size": 96, "label_smoothing": 0.1, "grad_clip": 10.0, "dropout": 0.3, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "salami128": {"sfreq": 128, "band_hz": [4.0, 38.0], "window_s": [0.0, 4.0], "norm": "ems", "car": false, "lr": 0.0005, "weight_decay": 0.0001, "scheduler": "plateau", "plateau_factor": 0.5, "plateau_patience": 30, "max_epochs": 600, "patience": 150, "batch_size": 96, "label_smoothing": 0.1, "grad_clip": 10.0, "dropout": 0.4, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "wide250": {"sfreq": 250, "band_hz": [4.0, 100.0], "window_s": [0.5, 4.0], "norm": "ems", "car": false, "lr": 0.0005, "weight_decay": 0.0001, "scheduler": "plateau", "plateau_factor": 0.5, "plateau_patience": 30, "max_epochs": 600, "patience": 150, "batch_size": 96, "label_smoothing": 0.1, "grad_clip": 10.0, "dropout": 0.4, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "wide250_full": {"sfreq": 250, "band_hz": [4.0, 100.0], "window_s": [0.0, 4.0], "norm": "ems", "car": false, "lr": 0.0005, "weight_decay": 0.0001, "scheduler": "plateau", "plateau_factor": 0.5, "plateau_patience": 30, "max_epochs": 600, "patience": 150, "batch_size": 96, "label_smoothing": 0.1, "grad_clip": 10.0, "dropout": 0.4, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}}
checkpoint_rule: "lowest validation loss, early stopping with patience; refit keeps final weights"
folds: "train on the official HGD training runs (last 25% = validation, chronological), refit on all training runs, test once on the official test runs"
seeds: [42, 43, 44]
```

Figures (75 topomaps: saliency per method/subject, group maps, ERD/ERS) copied to `2class\figures`.

## 4class

### T1. Test accuracy (%) per subject — chance 25.0%

Protocol: train on the official HGD training runs (last 25% = validation, chronological), refit on all training runs, test once on the official test runs. Subject accuracy = seed ensemble (mean softmax of 3 seeds); single seeds in T6. SD = across subjects (n = 14). Random = mean of the random-montage draws.

| Method | S01 | S02 | S03 | S04 | S05 | S06 | S07 | S08 | S09 | S10 | S11 | S12 | S13 | S14 | Mean | SD |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 22ch | 63.12 | 75.62 | 95.62 | 99.38 | 84.38 | 90.00 | 73.12 | 90.00 | 71.88 | 90.00 | 70.62 | 88.75 | 83.75 | 96.88 | 83.79 | 11.15 |
| Ours | 63.12 | 71.25 | 95.62 | 85.00 | 83.75 | 80.00 | 71.25 | 91.25 | 81.88 | 88.75 | 68.75 | 93.75 | 81.25 | 95.62 | 82.23 | 10.45 |
| CSP | 66.25 | 75.00 | 96.25 | 90.62 | 76.88 | 79.38 | 67.50 | 82.50 | 66.25 | 91.25 | 57.50 | 88.12 | 80.00 | 95.00 | 79.46 | 12.00 |
| RLF | 62.50 | 70.00 | 95.00 | 86.88 | 81.25 | 87.50 | 75.00 | 83.75 | 66.25 | 83.75 | 71.88 | 83.75 | 84.38 | 93.75 | 80.40 | 9.86 |
| MI | 52.50 | 68.75 | 96.88 | 94.38 | 87.50 | 85.00 | 78.75 | 84.38 | 75.00 | 86.25 | 70.62 | 91.88 | 80.00 | 93.75 | 81.83 | 12.13 |
| Fixed sensorimotor | 65.00 | 61.88 | 91.88 | 88.12 | 83.75 | 80.00 | 70.00 | 83.75 | 65.62 | 83.75 | 74.38 | 91.88 | 80.00 | 95.00 | 79.64 | 10.76 |
| ERD-only | 56.88 | 71.25 | 97.50 | 83.75 | 84.38 | 85.00 | 72.50 | 86.25 | 79.38 | 86.88 | 73.12 | 89.38 | 80.00 | 92.50 | 81.34 | 10.32 |
| Random (mean of draws) | 63.38 | 70.12 | 93.75 | 91.38 | 83.38 | 83.75 | 72.50 | 82.88 | 65.50 | 87.38 | 75.12 | 89.50 | 78.12 | 90.88 | 80.54 | 9.92 |

### T0. Data used per subject

Trials after the class selection of this experiment (training trials include the validation part, which is also used to fit the final model; the test trials are never used for any choice).

| Subject | Training trials (incl. validation) | Validation trials | Test trials | Test trials per class | Majority-class test accuracy (%) | Chance (%) |
|---|---|---|---|---|---|---|
| S01 | 320 | 80 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S02 | 813 | 203 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S03 | 880 | 220 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S04 | 897 | 224 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S05 | 720 | 180 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S06 | 880 | 220 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S07 | 880 | 220 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S08 | 654 | 164 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S09 | 880 | 220 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S10 | 880 | 220 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S11 | 880 | 220 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S12 | 880 | 220 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S13 | 800 | 200 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |
| S14 | 880 | 220 | 160 | feet 40, left_hand 40, rest 40, right_hand 40 | 25.00 | 25.00 |

### T2. Montages and profiles

Full list per subject in `T2_montages.csv` (all 12-channel montages are leave-one-subject-out).

| Method | Distinct montages across subjects | Most frequent montage |
|---|---|---|
| Ours | 14 | C3 C4 CP3 C2 CP1 C1 FC1 CP5 C6 CPz FC2 Pz |
| CSP | 14 | CP3 CP5 Pz CP6 C4 C3 CP2 C6 CP1 C5 FC6 FC5 |
| RLF | 8 | C2 C4 C1 C3 CP3 CP1 CP2 CP4 Pz CPz CP5 FC1 |
| MI | 10 | C2 C4 C1 CP3 C3 CP1 CP2 CP4 FC4 C6 CP6 FC1 |
| Fixed sensorimotor | 1 | FC3 FC1 FC2 FC4 C3 C1 Cz C2 C4 CP3 CPz CP4 |
| ERD-only | 13 | C4 C2 C1 C3 CP3 CP1 CP2 Pz CP6 CP4 CP5 CPz |

### T3. Equivalence of each 12-channel montage with all 22 channels (paired TOST)

Difference = montage − 22ch, in percentage points. Equivalent means the 90% CI lies inside the margin; it does not mean identical accuracy.

| Method | n | Mean diff (pp) | SD | 90% CI | TOST p | Equivalent (±6 pp) | Worst subject (pp) | Subjects losing >6 pp | Equivalent at margins (pp) |
|---|---|---|---|---|---|---|---|---|---|
| Ours | 14 | -1.56 | 5.78 | [-4.30, +1.18] | 0.0066 | yes | -14.38 | 2 | 5,6,8,10 |
| CSP | 14 | -4.33 | 4.84 | [-6.62, -2.04] | 0.1098 | no | -13.13 | 5 | 8,10 |
| RLF | 14 | -3.39 | 3.86 | [-5.22, -1.57] | 0.0126 | yes | -12.50 | 3 | 6,8,10 |
| MI | 14 | -1.96 | 4.71 | [-4.19, +0.26] | 0.0034 | yes | -10.62 | 2 | 5,6,8,10 |
| Fixed sensorimotor | 14 | -4.15 | 5.27 | [-6.64, -1.66] | 0.1059 | no | -13.75 | 6 | 8,10 |
| ERD-only | 14 | -2.46 | 5.31 | [-4.97, +0.06] | 0.0134 | yes | -15.62 | 2 | 5,6,8,10 |
| Random (mean of draws) | 14 | -3.25 | 3.69 | [-5.00, -1.50] | 0.0077 | yes | -8.00 | 4 | 5,6,8,10 |

### T4. Saliency montage (Ours) vs every other 12-channel montage

Positive = Ours more accurate. Holm correction across the comparisons in this table.

| Ours vs | n | Mean diff (pp) | 95% CI | paired t p | Holm | Wilcoxon p | Holm | Ours better / tie / worse |
|---|---|---|---|---|---|---|---|---|
| CSP | 14 | +2.77 | [-0.80, +6.34] | 0.1180 | 0.6382 | 0.1399 | 0.7557 | 9 / 0 / 5 |
| RLF | 14 | +1.83 | [-1.69, +5.35] | 0.2820 | 1.0000 | 0.4323 | 1.0000 | 9 / 0 / 5 |
| MI | 14 | +0.40 | [-2.86, +3.66] | 0.7942 | 1.0000 | 0.7533 | 1.0000 | 8 / 0 / 6 |
| Fixed sensorimotor | 14 | +2.59 | [-0.63, +5.81] | 0.1064 | 0.6382 | 0.1259 | 0.7557 | 9 / 2 / 3 |
| ERD-only | 14 | +0.89 | [-1.03, +2.82] | 0.3343 | 1.0000 | 0.2935 | 1.0000 | 8 / 1 / 5 |
| Random (mean of draws) | 14 | +1.69 | [-1.72, +5.09] | 0.3040 | 1.0000 | 0.3002 | 1.0000 | 9 / 0 / 5 |

### T5. Confusion, class balance and majority baseline (chance 25.0%)

Pooled over all subjects, folds and seeds; full matrices in `T5_confusion_matrices.csv`, per subject in `T5_confusion_per_subject.csv`. The last column flags models that collapsed to one class.

| Method | Pooled acc | Per-class recall | Predicted share per class | Mean majority-class acc | Folds predicting one class ≥90% |
|---|---|---|---|---|---|
| 22ch | 83.79 | feet 86.2, left_hand 83.2, rest 84.3, right_hand 81.4 | feet 23.8, left_hand 27.0, rest 22.8, right_hand 26.4 | 25.00 | 0 / 14 |
| Ours | 82.23 | feet 84.1, left_hand 83.4, rest 81.6, right_hand 79.8 | feet 23.2, left_hand 27.7, rest 22.8, right_hand 26.3 | 25.00 | 0 / 14 |
| CSP | 79.46 | feet 78.0, left_hand 77.3, rest 83.2, right_hand 79.3 | feet 21.9, left_hand 25.9, rest 23.6, right_hand 28.6 | 25.00 | 0 / 14 |
| RLF | 80.40 | feet 79.1, left_hand 79.8, rest 80.0, right_hand 82.7 | feet 22.0, left_hand 26.6, rest 22.8, right_hand 28.7 | 25.00 | 0 / 14 |
| MI | 81.83 | feet 82.3, left_hand 81.1, rest 80.5, right_hand 83.4 | feet 22.9, left_hand 26.6, rest 22.2, right_hand 28.3 | 25.00 | 0 / 14 |
| Fixed sensorimotor | 79.64 | feet 81.2, left_hand 81.6, rest 78.0, right_hand 77.7 | feet 22.5, left_hand 28.5, rest 21.9, right_hand 27.1 | 25.00 | 0 / 14 |
| ERD-only | 81.34 | feet 84.6, left_hand 80.5, rest 78.0, right_hand 82.1 | feet 24.2, left_hand 26.6, rest 22.1, right_hand 27.1 | 25.00 | 0 / 14 |
| Random (mean of draws) | 80.54 | feet 82.7, left_hand 81.6, rest 80.3, right_hand 77.6 | feet 23.2, left_hand 28.2, rest 22.1, right_hand 26.5 | 25.00 | 0 / 70 |

### T6. Seed stability

Grand mean of each single seed, before the seed ensemble used in T1.

| Method | Seeds | Grand mean per seed (%) | Mean across seeds | SD across seeds |
|---|---|---|---|---|
| 22ch | 3 | 42: 77.54, 43: 83.48, 44: 77.72 | 79.58 | 3.38 |
| Ours | 3 | 42: 78.39, 43: 79.29, 44: 78.88 | 78.85 | 0.45 |
| CSP | 3 | 42: 75.18, 43: 74.87, 44: 76.74 | 75.60 | 1.00 |
| RLF | 3 | 42: 78.75, 43: 75.04, 44: 76.92 | 76.90 | 1.85 |
| MI | 3 | 42: 80.27, 43: 76.29, 44: 79.42 | 78.66 | 2.09 |
| Fixed sensorimotor | 3 | 42: 76.56, 43: 77.46, 44: 76.47 | 76.83 | 0.54 |
| ERD-only | 3 | 42: 77.81, 43: 76.16, 44: 76.25 | 76.74 | 0.93 |
| Random (mean of draws) | 3 | 42: 76.40, 43: 76.44, 44: 77.01 | 76.62 | 0.34 |

### T7. Saliency vs ERD/ERS alignment (participant level)

magnitude / class_specific / lateralisation compare unsigned saliency with desynchronisation strength (−ERD) and are sign-invariant; `legacy_signed_LR` is the old statistic, shown only for comparison (its sign is not interpretable). Mean and CI via Fisher z. Per-subject values: `results/full22/alignment_metrics.json`.

| Attribution | Metric | Mean r (Fisher) | 95% CI | SD of r | n subjects |
|---|---|---|---|---|---|
| grad | magnitude_pearson | 0.132 | [-0.024, 0.282] | 0.258 | 14 |
| grad | class_specific_pearson | 0.111 | [-0.038, 0.255] | 0.244 | 14 |
| grad | lateralisation_pearson | 0.105 | [-0.066, 0.269] | 0.276 | 14 |
| grad | magnitude_spearman | 0.186 | [0.054, 0.311] | 0.218 | 14 |
| grad | class_specific_spearman | 0.201 | [0.106, 0.292] | 0.154 | 14 |
| grad | lateralisation_spearman | 0.075 | [-0.089, 0.235] | 0.259 | 14 |
| grad | legacy_signed_LR_pearson | 0.062 | [-0.089, 0.211] | 0.246 | 14 |
| grad_x_input | magnitude_pearson | 0.314 | [0.153, 0.459] | 0.264 | 14 |
| grad_x_input | class_specific_pearson | 0.191 | [0.036, 0.337] | 0.249 | 14 |
| grad_x_input | lateralisation_pearson | -0.102 | [-0.277, 0.080] | 0.302 | 14 |
| grad_x_input | magnitude_spearman | 0.187 | [-0.052, 0.406] | 0.353 | 14 |
| grad_x_input | class_specific_spearman | 0.100 | [-0.032, 0.229] | 0.215 | 14 |
| grad_x_input | lateralisation_spearman | -0.173 | [-0.349, 0.014] | 0.301 | 14 |
| grad_x_input | legacy_signed_LR_pearson | 0.175 | [0.077, 0.270] | 0.165 | 14 |
| integrated_gradients | magnitude_pearson | 0.315 | [0.148, 0.464] | 0.271 | 14 |
| integrated_gradients | class_specific_pearson | 0.130 | [-0.033, 0.287] | 0.260 | 14 |
| integrated_gradients | lateralisation_pearson | -0.283 | [-0.482, -0.056] | 0.339 | 14 |
| integrated_gradients | magnitude_spearman | 0.201 | [-0.067, 0.443] | 0.381 | 14 |
| integrated_gradients | class_specific_spearman | 0.048 | [-0.097, 0.191] | 0.237 | 14 |
| integrated_gradients | lateralisation_spearman | -0.261 | [-0.452, -0.047] | 0.324 | 14 |
| integrated_gradients | legacy_signed_LR_pearson | 0.161 | [0.050, 0.267] | 0.186 | 14 |
| smoothgrad | magnitude_pearson | 0.135 | [-0.026, 0.289] | 0.264 | 14 |
| smoothgrad | class_specific_pearson | 0.123 | [-0.030, 0.269] | 0.249 | 14 |
| smoothgrad | lateralisation_pearson | 0.112 | [-0.054, 0.272] | 0.270 | 14 |
| smoothgrad | magnitude_spearman | 0.192 | [0.055, 0.323] | 0.228 | 14 |
| smoothgrad | class_specific_spearman | 0.200 | [0.100, 0.296] | 0.164 | 14 |
| smoothgrad | lateralisation_spearman | 0.083 | [-0.056, 0.218] | 0.221 | 14 |
| smoothgrad | legacy_signed_LR_pearson | 0.062 | [-0.087, 0.208] | 0.242 | 14 |

### T7b. Correlations as computed by the original scripts

corr(saliency, ERD_L / ERD_R / ERD_(L−R) / ERD_comb) and corr(saliency, plain-gradient saliency), participant level. Kept so the earlier numbers can be compared; an unsigned map is correlated with a signed one, so the sign is not 'agreement' (use T7).

| Attribution | Correlation | Mean r (Fisher) | 95% CI | n subjects |
|---|---|---|---|---|
| grad | ERD_L_pearson | -0.161 | [-0.307, -0.008] | 14 |
| grad | ERD_L_spearman | -0.224 | [-0.342, -0.100] | 14 |
| grad | ERD_R_pearson | -0.160 | [-0.298, -0.015] | 14 |
| grad | ERD_R_spearman | -0.222 | [-0.330, -0.107] | 14 |
| grad | ERD_LR_pearson | 0.062 | [-0.089, 0.211] | 14 |
| grad | ERD_LR_spearman | 0.059 | [-0.089, 0.205] | 14 |
| grad | ERD_comb_pearson | -0.161 | [-0.305, -0.008] | 14 |
| grad | ERD_comb_spearman | -0.238 | [-0.354, -0.114] | 14 |
| grad | vs_grad_pearson | 1.000 | [1.000, 1.000] | 14 |
| grad | vs_grad_spearman | 1.000 | [1.000, 1.000] | 14 |
| grad_x_input | ERD_L_pearson | -0.262 | [-0.420, -0.089] | 14 |
| grad_x_input | ERD_L_spearman | -0.196 | [-0.379, 0.001] | 14 |
| grad_x_input | ERD_R_pearson | -0.322 | [-0.448, -0.184] | 14 |
| grad_x_input | ERD_R_spearman | -0.276 | [-0.437, -0.097] | 14 |
| grad_x_input | ERD_LR_pearson | 0.175 | [0.077, 0.270] | 14 |
| grad_x_input | ERD_LR_spearman | 0.211 | [0.061, 0.353] | 14 |
| grad_x_input | ERD_comb_pearson | -0.305 | [-0.444, -0.152] | 14 |
| grad_x_input | ERD_comb_spearman | -0.262 | [-0.435, -0.072] | 14 |
| grad_x_input | vs_grad_pearson | 0.544 | [-0.046, 0.852] | 14 |
| grad_x_input | vs_grad_spearman | 0.488 | [-0.020, 0.795] | 14 |
| integrated_gradients | ERD_L_pearson | -0.265 | [-0.425, -0.088] | 14 |
| integrated_gradients | ERD_L_spearman | -0.186 | [-0.370, 0.012] | 14 |
| integrated_gradients | ERD_R_pearson | -0.325 | [-0.452, -0.185] | 14 |
| integrated_gradients | ERD_R_spearman | -0.281 | [-0.448, -0.096] | 14 |
| integrated_gradients | ERD_LR_pearson | 0.161 | [0.050, 0.267] | 14 |
| integrated_gradients | ERD_LR_spearman | 0.220 | [0.048, 0.380] | 14 |
| integrated_gradients | ERD_comb_pearson | -0.309 | [-0.448, -0.155] | 14 |
| integrated_gradients | ERD_comb_spearman | -0.261 | [-0.442, -0.060] | 14 |
| integrated_gradients | vs_grad_pearson | 0.342 | [0.040, 0.587] | 14 |
| integrated_gradients | vs_grad_spearman | 0.284 | [0.034, 0.500] | 14 |
| smoothgrad | ERD_L_pearson | -0.164 | [-0.313, -0.007] | 14 |
| smoothgrad | ERD_L_spearman | -0.237 | [-0.361, -0.105] | 14 |
| smoothgrad | ERD_R_pearson | -0.162 | [-0.303, -0.014] | 14 |
| smoothgrad | ERD_R_spearman | -0.227 | [-0.340, -0.107] | 14 |
| smoothgrad | ERD_LR_pearson | 0.062 | [-0.087, 0.208] | 14 |
| smoothgrad | ERD_LR_spearman | 0.052 | [-0.097, 0.198] | 14 |
| smoothgrad | ERD_comb_pearson | -0.163 | [-0.312, -0.007] | 14 |
| smoothgrad | ERD_comb_spearman | -0.247 | [-0.368, -0.117] | 14 |
| smoothgrad | vs_grad_pearson | 0.999 | [0.999, 1.000] | 14 |
| smoothgrad | vs_grad_spearman | 0.999 | [0.994, 1.000] | 14 |

### T10. EXPLORATORY: saliency vs other physiological maps

Curiosity only — not used for any choice; the paper's alignment is T7. Saliency = mean of the four attribution maps (`mean4`); per method in `T10_physiology_all_methods.csv`. r = corr(saliency, map), |map| = corr(saliency, |map|), class-specific = mean of corr(saliency_L, |map_L|) and corr(saliency_R, |map_R|). Fisher-z mean over subjects. Group maps: `figures/physiology_maps_group.png`.

| Map | Pearson r | 95% CI | Pearson r (|map|) | Spearman r | Spearman r (|map|) | n |
|---|---|---|---|---|---|---|
| ERD_theta_L | -0.089 | [-0.233, 0.059] | 0.124 | -0.036 | 0.134 | 14 |
| ERD_theta_R | -0.088 | [-0.271, 0.100] | 0.024 | -0.083 | 0.042 | 14 |
| ERD_theta_mag | 0.053 | [-0.101, 0.205] | 0.053 | 0.071 | 0.071 | 14 |
| ERD_mu_L | -0.240 | [-0.397, -0.069] | 0.239 | -0.217 | 0.216 | 14 |
| ERD_mu_R | -0.252 | [-0.378, -0.116] | 0.157 | -0.268 | 0.118 | 14 |
| ERD_mu_mag | 0.182 | [0.024, 0.330] | 0.182 | 0.144 | 0.144 | 14 |
| ERD_beta_L | -0.365 | [-0.469, -0.252] | 0.406 | -0.374 | 0.394 | 14 |
| ERD_beta_R | -0.397 | [-0.499, -0.284] | 0.381 | -0.418 | 0.346 | 14 |
| ERD_beta_mag | 0.384 | [0.246, 0.506] | 0.384 | 0.354 | 0.354 | 14 |
| ERS_beta_rebound_L | -0.174 | [-0.325, -0.014] | 0.227 | -0.127 | 0.189 | 14 |
| ERS_beta_rebound_R | -0.124 | [-0.300, 0.059] | 0.176 | -0.134 | 0.166 | 14 |
| ERS_beta_rebound_mag | 0.223 | [0.058, 0.375] | 0.223 | 0.209 | 0.209 | 14 |
| ERD_lowgamma_L | -0.252 | [-0.421, -0.067] | 0.274 | -0.285 | 0.298 | 14 |
| ERD_lowgamma_R | -0.300 | [-0.439, -0.148] | 0.232 | -0.372 | 0.262 | 14 |
| ERD_lowgamma_mag | 0.231 | [0.059, 0.389] | 0.231 | 0.266 | 0.266 | 14 |
| ERD_highgamma_L | 0.008 | [-0.204, 0.219] | 0.165 | 0.050 | 0.199 | 14 |
| ERD_highgamma_R | 0.157 | [-0.043, 0.345] | 0.016 | 0.136 | 0.024 | 14 |
| ERD_highgamma_mag | 0.066 | [-0.124, 0.251] | 0.066 | 0.088 | 0.088 | 14 |
| logpow_8_30 | 0.174 | [0.040, 0.301] | -0.097 | 0.116 | -0.040 | 14 |
| r2_signed | -0.132 | [-0.287, 0.028] | 0.092 | -0.119 | 0.136 | 14 |
| r2_abs | 0.092 | [-0.096, 0.273] | 0.092 | 0.136 | 0.136 | 14 |
| TFR_ERD_dB_L | -0.365 | [-0.472, -0.248] | 0.397 | -0.359 | 0.366 | 14 |
| TFR_ERD_dB_R | -0.396 | [-0.499, -0.283] | 0.360 | -0.394 | 0.327 | 14 |
| TFR_ERD_dB_mag | 0.368 | [0.208, 0.508] | 0.368 | 0.339 | 0.339 | 14 |
| ITC_4_30 | 0.166 | [-0.021, 0.342] | 0.166 | 0.200 | 0.200 | 14 |
| ERP_abs_0.2_0.8 | 0.037 | [-0.146, 0.219] | 0.037 | 0.059 | 0.059 | 14 |
| SlowPot_0.5_3 | -0.153 | [-0.272, -0.030] | 0.102 | -0.142 | 0.118 | 14 |
| ERD_beta_classspecific | — | — | 0.308 [0.174, 0.431] | — | 0.259 | 14 |
| ERD_highgamma_classspecific | — | — | 0.123 [-0.006, 0.249] | — | 0.168 | 14 |
| ERD_lowgamma_classspecific | — | — | 0.197 [0.055, 0.331] | — | 0.176 | 14 |
| ERD_mu_classspecific | — | — | 0.118 [-0.010, 0.242] | — | 0.073 | 14 |
| ERD_theta_classspecific | — | — | 0.066 [-0.062, 0.193] | — | 0.086 | 14 |
| ERS_beta_rebound_classspecific | — | — | 0.145 [0.004, 0.280] | — | 0.094 | 14 |
| TFR_ERD_dB_classspecific | — | — | 0.261 [0.132, 0.381] | — | 0.226 | 14 |

### T8a. Faithfulness: deletion test on the test trials

Accuracy drop (intact − channels removed), mean ± SD across subjects. Ranking from validation saliency; removal = channel set to its standardised mean. A faithful ranking gives the largest drop for top-ranked channels.

| Removed channels k | Drop: top-ranked (pp) | Drop: random (pp) | Drop: bottom-ranked (pp) | top vs random p | top vs bottom p |
|---|---|---|---|---|---|
| 2 | +28.17 ± 10.61 | +12.76 ± 5.70 | +3.59 ± 2.93 | <0.0001 | <0.0001 |
| 4 | +35.67 ± 12.31 | +22.70 ± 10.97 | +10.89 ± 8.11 | <0.0001 | <0.0001 |
| 6 | +38.07 ± 9.91 | +28.43 ± 10.10 | +16.31 ± 12.00 | <0.0001 | <0.0001 |

### T8b. Model-randomisation sanity check

Similarity between saliency of the trained model and of an untrained model. High values mean the map reflects the input more than what the network learned.

| Attribution | Spearman(trained, untrained model) | 95% CI | n subjects |
|---|---|---|---|
| grad | 0.040 | [-0.012, 0.092] | 14 |
| grad_x_input | 0.494 | [0.366, 0.604] | 14 |
| integrated_gradients | 0.524 | [0.417, 0.618] | 14 |
| smoothgrad | 0.036 | [-0.016, 0.087] | 14 |

### T9. Configuration

Full snapshot: `T9_config.json`.

Training profile chosen on validation data only, leave-one-subject-out (unanimous: False): S01=original, S02=original, S03=original, S04=original, S05=original, S06=original, S07=original, S08=original, S09=ems, S10=original, S11=original, S12=original, S13=original, S14=original

| Profile | Mean validation accuracy (%) |
|---|---|
| original | 80.19 |
| ems | 79.16 |
| salami128 | 73.23 |

```
model: "EEGITNet"
dataset: "Schirrmeister2017"
sfreq_hz: "per profile (profiles[*].sfreq)"
profiles: {"original": {"sfreq": 100, "band_hz": [4.0, 38.0], "window_s": [0.0, 4.0], "norm": null, "car": false, "lr": 0.0005, "weight_decay": 0.0001, "scheduler": "plateau", "plateau_factor": 0.5, "plateau_patience": 30, "max_epochs": 600, "patience": 150, "batch_size": 96, "label_smoothing": 0.1, "grad_clip": 10.0, "dropout": 0.3, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "ems": {"sfreq": 100, "band_hz": [4.0, 38.0], "window_s": [0.0, 4.0], "norm": "ems", "car": false, "lr": 0.0005, "weight_decay": 0.0001, "scheduler": "plateau", "plateau_factor": 0.5, "plateau_patience": 30, "max_epochs": 600, "patience": 150, "batch_size": 96, "label_smoothing": 0.1, "grad_clip": 10.0, "dropout": 0.3, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "salami128": {"sfreq": 128, "band_hz": [4.0, 38.0], "window_s": [0.0, 4.0], "norm": "ems", "car": false, "lr": 0.0005, "weight_decay": 0.0001, "scheduler": "plateau", "plateau_factor": 0.5, "plateau_patience": 30, "max_epochs": 600, "patience": 150, "batch_size": 96, "label_smoothing": 0.1, "grad_clip": 10.0, "dropout": 0.4, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "wide250": {"sfreq": 250, "band_hz": [4.0, 100.0], "window_s": [0.5, 4.0], "norm": "ems", "car": false, "lr": 0.0005, "weight_decay": 0.0001, "scheduler": "plateau", "plateau_factor": 0.5, "plateau_patience": 30, "max_epochs": 600, "patience": 150, "batch_size": 96, "label_smoothing": 0.1, "grad_clip": 10.0, "dropout": 0.4, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}, "wide250_full": {"sfreq": 250, "band_hz": [4.0, 100.0], "window_s": [0.0, 4.0], "norm": "ems", "car": false, "lr": 0.0005, "weight_decay": 0.0001, "scheduler": "plateau", "plateau_factor": 0.5, "plateau_patience": 30, "max_epochs": 600, "patience": 150, "batch_size": 96, "label_smoothing": 0.1, "grad_clip": 10.0, "dropout": 0.4, "augment": false, "select_on": "val_acc", "min_select_epoch": 20}}
checkpoint_rule: "lowest validation loss, early stopping with patience; refit keeps final weights"
folds: "train on the official HGD training runs (last 25% = validation, chronological), refit on all training runs, test once on the official test runs"
seeds: [42, 43, 44]
```

Figures (75 topomaps: saliency per method/subject, group maps, ERD/ERS) copied to `4class\figures`.
