# Cross-model summary — EEGNetV4/PhysioNet, EEGItNet/PhysioNet, Deep4net/PhysioNet, EEGConformer/PhysioNet

Generated 2026-10-24 18:39. Per-model details: `<model folder>/report*/REPORT.md` (results folder `<class>/results_session/`).

## C1. Test accuracy (%), mean ± SD across subjects

| Model | Class | Full montage (22ch BNCI/HGD, 64ch PhysioNet) | Ours | CSP | RLF | MI | Fixed sensorimotor | ERD-only | Random (mean of draws) |
|---|---|---|---|---|---|---|---|---|---|
| EEGNetV4 | 2class | 57.27 ± 15.41 | 55.43 ± 14.83 | 56.00 ± 14.37 | 56.38 ± 13.33 | 56.13 ± 13.83 | 54.03 ± 12.87 | 53.78 ± 12.24 | 53.96 ± 9.81 |
| EEGNetV4 | 4class | 32.60 ± 12.15 | 30.83 ± 11.15 | 30.38 ± 10.70 | 29.97 ± 12.60 | 28.92 ± 12.18 | 30.54 ± 11.64 | 30.32 ± 9.42 | 30.13 ± 8.33 |
| EEGItNet | 2class | 54.54 ± 13.13 | 53.02 ± 11.71 | 55.24 ± 12.36 | 56.32 ± 12.05 | 55.62 ± 11.65 | 53.02 ± 10.99 | 54.35 ± 12.26 | 54.46 ± 9.37 |
| EEGItNet | 4class | 29.49 ± 9.94 | 28.44 ± 7.21 | 28.10 ± 8.00 | 28.95 ± 9.54 | 29.71 ± 8.86 | 27.97 ± 8.98 | 29.49 ± 7.63 | 29.14 ± 6.05 |
| Deep4net | 2class | — | 50.79 ± 7.36 | 51.30 ± 8.83 | 52.13 ± 8.46 | 52.95 ± 8.61 | 53.65 ± 9.58 | 52.51 ± 8.20 | 51.82 ± 6.21 |
| Deep4net | 4class | 27.68 ± 8.81 | 27.94 ± 9.27 | 27.40 ± 7.95 | 28.13 ± 8.89 | 28.83 ± 9.54 | 28.29 ± 8.74 | 28.16 ± 7.31 | 28.14 ± 7.21 |
| EEGConformer | 2class | 64.00 ± 15.57 | 58.98 ± 14.01 | 57.84 ± 14.89 | 60.70 ± 15.30 | 60.19 ± 14.57 | 60.32 ± 16.31 | 61.90 ± 14.46 | 60.66 ± 12.01 |
| EEGConformer | 4class | 37.52 ± 13.71 | 33.81 ± 13.05 | 31.81 ± 10.94 | 34.57 ± 13.61 | 33.62 ± 13.60 | 33.78 ± 15.20 | 34.51 ± 12.34 | 34.93 ± 10.95 |

## C2. Saliency–ERD correlations (Pearson, Fisher mean over subjects)

First three: sign-invariant metrics used in the paper. Last two: as in the original scripts.

| Model | Class | Attribution | magnitude r | class-specific r | lateralisation r | orig ERD_(L−R) r | orig ERD_comb r |
|---|---|---|---|---|---|---|---|
| EEGNetV4 | 2class | grad | 0.017 | -0.013 | -0.015 | 0.011 | 0.014 |
| EEGNetV4 | 2class | grad_x_input | -0.008 | -0.002 | -0.103 | 0.005 | -0.036 |
| EEGNetV4 | 2class | integrated_gradients | -0.007 | -0.002 | -0.100 | 0.007 | -0.036 |
| EEGNetV4 | 2class | smoothgrad | 0.017 | -0.013 | -0.016 | 0.011 | 0.014 |
| EEGNetV4 | 4class | grad | -0.036 | 0.007 | 0.011 | -0.007 | -0.010 |
| EEGNetV4 | 4class | grad_x_input | -0.050 | 0.002 | -0.085 | -0.009 | -0.049 |
| EEGNetV4 | 4class | integrated_gradients | -0.050 | 0.002 | -0.082 | -0.007 | -0.049 |
| EEGNetV4 | 4class | smoothgrad | -0.036 | 0.006 | 0.011 | -0.007 | -0.010 |
| EEGItNet | 2class | grad | -0.013 | 0.013 | -0.012 | 0.008 | -0.019 |
| EEGItNet | 2class | grad_x_input | -0.052 | 0.009 | -0.165 | -0.002 | -0.052 |
| EEGItNet | 2class | integrated_gradients | -0.053 | 0.008 | -0.165 | -0.001 | -0.049 |
| EEGItNet | 2class | smoothgrad | -0.013 | 0.013 | -0.012 | 0.008 | -0.019 |
| EEGItNet | 4class | grad | -0.007 | 0.010 | -0.018 | -0.008 | -0.013 |
| EEGItNet | 4class | grad_x_input | -0.046 | -0.042 | -0.113 | 0.003 | 0.021 |
| EEGItNet | 4class | integrated_gradients | -0.047 | -0.042 | -0.098 | 0.005 | 0.019 |
| EEGItNet | 4class | smoothgrad | -0.007 | 0.010 | -0.018 | -0.008 | -0.013 |
| Deep4net | 4class | grad | 0.008 | -0.041 | -0.054 | -0.007 | 0.042 |
| Deep4net | 4class | grad_x_input | -0.012 | -0.064 | -0.183 | -0.008 | 0.018 |
| Deep4net | 4class | integrated_gradients | -0.009 | -0.063 | -0.186 | -0.012 | 0.019 |
| Deep4net | 4class | smoothgrad | 0.008 | -0.041 | -0.059 | -0.007 | 0.042 |
| EEGConformer | 2class | grad | -0.018 | -0.036 | -0.001 | 0.034 | 0.042 |
| EEGConformer | 2class | grad_x_input | -0.035 | -0.027 | -0.096 | 0.030 | 0.015 |
| EEGConformer | 2class | integrated_gradients | -0.029 | -0.027 | -0.138 | 0.025 | 0.017 |
| EEGConformer | 2class | smoothgrad | -0.018 | -0.035 | -0.003 | 0.034 | 0.041 |
| EEGConformer | 4class | grad | -0.069 | -0.054 | 0.020 | 0.027 | 0.062 |
| EEGConformer | 4class | grad_x_input | -0.085 | -0.056 | -0.044 | 0.021 | 0.046 |
| EEGConformer | 4class | integrated_gradients | -0.075 | -0.042 | -0.032 | 0.018 | 0.040 |
| EEGConformer | 4class | smoothgrad | -0.069 | -0.054 | 0.022 | 0.027 | 0.063 |

## C3. EXPLORATORY: corr(mean saliency, physiological map), Pearson, Fisher mean

Curiosity only; not used anywhere in the pipeline.

| Map | Deep4net 2class | Deep4net 4class | EEGConformer 2class | EEGConformer 4class | EEGItNet 2class | EEGItNet 4class | EEGNetV4 2class | EEGNetV4 4class |
|---|---|---|---|---|---|---|---|---|
| ERD_theta_L | -0.090 | -0.062 | -0.026 | 0.019 | -0.050 | -0.004 | -0.046 | 0.000 |
| ERD_theta_R | -0.038 | -0.030 | -0.047 | -0.033 | -0.043 | -0.002 | -0.003 | -0.037 |
| ERD_theta_mag | -0.097 | -0.025 | -0.058 | -0.050 | -0.036 | -0.014 | -0.045 | -0.080 |
| ERD_mu_L | -0.059 | 0.017 | 0.032 | 0.034 | -0.029 | 0.000 | -0.006 | -0.020 |
| ERD_mu_R | 0.003 | 0.050 | 0.009 | 0.033 | -0.030 | 0.004 | 0.001 | -0.025 |
| ERD_mu_mag | -0.010 | 0.011 | -0.043 | -0.082 | -0.031 | -0.030 | 0.002 | -0.044 |
| ERD_beta_L | -0.033 | 0.021 | 0.024 | 0.066 | -0.023 | 0.007 | 0.009 | -0.018 |
| ERD_beta_R | 0.029 | 0.022 | 0.035 | 0.040 | -0.004 | 0.017 | -0.005 | 0.017 |
| ERD_beta_mag | -0.038 | -0.006 | 0.011 | -0.032 | -0.012 | -0.008 | -0.018 | -0.029 |
| ERS_beta_rebound_L | -0.014 | 0.008 | 0.016 | 0.032 | -0.021 | -0.015 | 0.010 | -0.033 |
| ERS_beta_rebound_R | -0.013 | 0.009 | -0.007 | 0.015 | -0.036 | -0.014 | -0.013 | -0.006 |
| ERS_beta_rebound_mag | 0.017 | 0.002 | 0.011 | -0.013 | 0.006 | 0.005 | 0.008 | -0.016 |
| ERD_lowgamma_L | -0.024 | 0.007 | -0.006 | 0.010 | 0.010 | 0.003 | -0.012 | -0.004 |
| ERD_lowgamma_R | -0.024 | -0.002 | 0.045 | 0.020 | 0.001 | 0.019 | 0.011 | 0.019 |
| ERD_lowgamma_mag | -0.004 | -0.002 | 0.040 | 0.031 | -0.003 | 0.003 | -0.008 | -0.007 |
| logpow_8_30 | 0.034 | 0.044 | -0.139 | -0.157 | 0.003 | -0.034 | 0.010 | -0.032 |
| r2_signed | 0.063 | 0.053 | 0.026 | 0.005 | 0.008 | 0.003 | -0.009 | 0.018 |
| r2_abs | 0.028 | -0.017 | 0.039 | -0.029 | 0.004 | 0.019 | 0.013 | 0.004 |
| TFR_ERD_dB_L | -0.060 | -0.004 | 0.022 | 0.052 | -0.031 | 0.004 | -0.001 | -0.020 |
| TFR_ERD_dB_R | 0.005 | 0.019 | 0.019 | 0.032 | -0.018 | 0.010 | -0.008 | -0.006 |
| TFR_ERD_dB_mag | -0.043 | -0.002 | -0.004 | -0.051 | -0.030 | -0.027 | -0.013 | -0.041 |
| ITC_4_30 | -0.003 | -0.030 | -0.074 | -0.116 | -0.024 | -0.013 | -0.018 | -0.021 |
| ERP_abs_0.2_0.8 | -0.077 | -0.069 | -0.158 | -0.176 | -0.017 | -0.014 | -0.055 | -0.059 |
| SlowPot_0.5_3 | -0.021 | -0.002 | -0.012 | -0.020 | -0.032 | -0.027 | -0.023 | -0.022 |
