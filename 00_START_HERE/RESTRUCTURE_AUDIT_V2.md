# Restructure Audit V2

Second pass used Git object bytes from `git show HEAD:<path>` for files previously under `90_UNASSIGNED_REVIEW/`, avoiding Windows working-tree LF-to-CRLF hash drift.

## Summary
- Original unassigned scientific file count: 95
- Second-pass resolved source file count: 95
- Second-pass restored manifest target count: 110
- Remaining genuinely unassigned scientific file count: 0
- Reason for original hash mismatch: Windows text checkout converted LF manifest bytes to CRLF working-tree bytes before SHA256 calculation.
- Restored E01 files: 14
- Restored E02 files: 33
- Restored E03 files: 13
- Restored E04 files: 7
- Restored E05 files: 17
- Restored E06 files: 14
- E07 status: RUNNING; canonical notebook present
- Manifest paths still missing: 167
- Files only available inside ZIP archives by basename evidence: 165
- External GB reproducibility assets still required: 0
- Manifest paths missing and not found in repository/ZIP by this audit: 2
- Manifest paths with wrong Git-object SHA after restore: 0

## Completion Checks
- FINAL_FREEZE_COMPLETE: expected_rows=675, actual_rows=675
- FINAL_N10_COMPLETE: master_expected=7560, master_actual=7560, al_expected=17280, al_actual=17280, systems=14, seeds=10, performance_based_seed_exclusions=[]
- AL_SSL_INTERACTION_COMPLETE: expected T0 states=50, actual T0 states=50, result_rows=720

## Resolved Files
- `90_UNASSIGNED_REVIEW/ACTIVE_LEARNING_full_matrix_n10.csv` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/ACTIVE_LEARNING_full_matrix_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/ACTIVE_LEARNING_summary_n10.csv` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/ACTIVE_LEARNING_summary_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/AL_SSL_INTERACTION_COMPLETE.json` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/AL_SSL_INTERACTION_COMPLETE.json` (git mv)
- `90_UNASSIGNED_REVIEW/AL_SSL_INTERACTION_COMPLETE.json` -> `06_LOGS_AUDITS/AL_SSL_INTERACTION_COMPLETE.json` (git blob copy)
- `90_UNASSIGNED_REVIEW/AL_SSL_INTERACTION_PROGRESS.json` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/audit/AL_SSL_INTERACTION_PROGRESS.json` (git mv)
- `90_UNASSIGNED_REVIEW/AL_SSL_INTERACTION_results_long.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/AL_SSL_INTERACTION_results_long.csv` (git mv)
- `90_UNASSIGNED_REVIEW/AL_SSL_INTERACTION_statistics_n10.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/AL_SSL_INTERACTION_statistics_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/ap_equal_n_sensitivity_results.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/ap_equal_n_sensitivity_results.csv` (git mv)
- `90_UNASSIGNED_REVIEW/ap_shift_corrected_prevalence_matched.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/ap_shift_corrected_prevalence_matched.csv` (git mv)
- `90_UNASSIGNED_REVIEW/ap_shift_equal_n_sensitivity.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/ap_shift_equal_n_sensitivity.csv` (git mv)
- `90_UNASSIGNED_REVIEW/artifact_audit.json` -> `04_RESULTS/E01_CORE_FREEZE/artifact_audit.json` (git mv)
- `90_UNASSIGNED_REVIEW/artifact_audit.json` -> `06_LOGS_AUDITS/artifact_audit.json` (git blob copy)
- `90_UNASSIGNED_REVIEW/b0_structural_feature_columns.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/b0_structural_feature_columns.csv` (git mv)
- `90_UNASSIGNED_REVIEW/b0_train_only_tuning.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/b0_train_only_tuning.csv` (git mv)
- `90_UNASSIGNED_REVIEW/best_classifier_params.json` -> `04_RESULTS/E01_CORE_FREEZE/best_classifier_params.json` (git mv)
- `90_UNASSIGNED_REVIEW/cascade_results.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/cascade_results.csv` (git mv)
- `90_UNASSIGNED_REVIEW/CASCADE_STAGE1_JUSTIFICATION.csv` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/CASCADE_STAGE1_JUSTIFICATION.csv` (git mv)
- `90_UNASSIGNED_REVIEW/CASCADE_stage1_sensitivity_n10.csv` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/CASCADE_stage1_sensitivity_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/CASCADE_stage1_sensitivity_summary_n10.csv` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/CASCADE_stage1_sensitivity_summary_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/cascade_summary.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/cascade_summary.csv` (git mv)
- `90_UNASSIGNED_REVIEW/classifier_tuning.csv` -> `04_RESULTS/E01_CORE_FREEZE/classifier_tuning.csv` (git mv)
- `90_UNASSIGNED_REVIEW/configuration.json` -> `04_RESULTS/E01_CORE_FREEZE/configuration.json` (git mv)
- `90_UNASSIGNED_REVIEW/contrastive_training_history.csv` -> `04_RESULTS/E01_CORE_FREEZE/contrastive_training_history.csv` (git mv)
- `90_UNASSIGNED_REVIEW/DAPT_E2E_training_history_seed42.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/DAPT_E2E_training_history_seed42.csv` (git mv)
- `90_UNASSIGNED_REVIEW/DAPT_E2E_training_history_seed52.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/DAPT_E2E_training_history_seed52.csv` (git mv)
- `90_UNASSIGNED_REVIEW/DAPT_E2E_training_history_seed62.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/DAPT_E2E_training_history_seed62.csv` (git mv)
- `90_UNASSIGNED_REVIEW/DAPT_E2E_training_history_seed72.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/DAPT_E2E_training_history_seed72.csv` (git mv)
- `90_UNASSIGNED_REVIEW/DAPT_E2E_training_history_seed82.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/DAPT_E2E_training_history_seed82.csv` (git mv)
- `90_UNASSIGNED_REVIEW/DAPT_T0_gaps_by_AL_strategy.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/DAPT_T0_gaps_by_AL_strategy.csv` (git mv)
- `90_UNASSIGNED_REVIEW/effect_confidence_intervals.csv` -> `04_RESULTS/E01_CORE_FREEZE/effect_confidence_intervals.csv` (git mv)
- `90_UNASSIGNED_REVIEW/error_complementarity.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/error_complementarity.csv` (git mv)
- `90_UNASSIGNED_REVIEW/error_complementarity_summary.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/error_complementarity_summary.csv` (git mv)
- `90_UNASSIGNED_REVIEW/error_feature_profiles_seed42.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/error_feature_profiles_seed42.csv` (git mv)
- `90_UNASSIGNED_REVIEW/figure_manifest.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/figures/figure_manifest.csv` (git mv)
- `90_UNASSIGNED_REVIEW/FINAL_FREEZE_COMPLETE.json` -> `04_RESULTS/E01_CORE_FREEZE/FINAL_FREEZE_COMPLETE.json` (git mv)
- `90_UNASSIGNED_REVIEW/FINAL_FREEZE_COMPLETE.json` -> `06_LOGS_AUDITS/FINAL_FREEZE_COMPLETE.json` (git blob copy)
- `90_UNASSIGNED_REVIEW/FINAL_N10_COMPLETE.json` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/FINAL_N10_COMPLETE.json` (git mv)
- `90_UNASSIGNED_REVIEW/FINAL_N10_COMPLETE.json` -> `06_LOGS_AUDITS/FINAL_N10_COMPLETE.json` (git blob copy)
- `90_UNASSIGNED_REVIEW/freeze_corrected_results.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_corrected_results.csv` (git mv)
- `90_UNASSIGNED_REVIEW/freeze_corrected_summary.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_corrected_summary.csv` (git mv)
- `90_UNASSIGNED_REVIEW/HYBRID_FREEZE_EXTENSION_COMPLETE.json` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/HYBRID_FREEZE_EXTENSION_COMPLETE.json` (git mv)
- `90_UNASSIGNED_REVIEW/HYBRID_FREEZE_EXTENSION_COMPLETE.json` -> `06_LOGS_AUDITS/HYBRID_FREEZE_EXTENSION_COMPLETE.json` (git blob copy)
- `90_UNASSIGNED_REVIEW/label_budget_audit.csv` -> `04_RESULTS/E01_CORE_FREEZE/label_budget_audit.csv` (git mv)
- `90_UNASSIGNED_REVIEW/label_budget_audit.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/label_budget_audit.csv` (git blob copy)
- `90_UNASSIGNED_REVIEW/LOOP_acquisition_audit.csv` -> `04_RESULTS/E04_PRODUCTIVE_AL/LOOP_acquisition_audit.csv` (git mv)
- `90_UNASSIGNED_REVIEW/LOOP_acquisition_audit.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/LOOP_acquisition_audit.csv` (git blob copy)
- `90_UNASSIGNED_REVIEW/LOOP_annotation_efficiency.csv` -> `04_RESULTS/E04_PRODUCTIVE_AL/LOOP_annotation_efficiency.csv` (git mv)
- `90_UNASSIGNED_REVIEW/LOOP_annotation_efficiency.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/LOOP_annotation_efficiency.csv` (git blob copy)
- `90_UNASSIGNED_REVIEW/LOOP_results_long.csv` -> `04_RESULTS/E04_PRODUCTIVE_AL/LOOP_results_long.csv` (git mv)
- `90_UNASSIGNED_REVIEW/LOOP_results_long.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/LOOP_results_long.csv` (git blob copy)
- `90_UNASSIGNED_REVIEW/LOOP_SSL_refresh_ablation.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/LOOP_SSL_refresh_ablation.csv` (git mv)
- `90_UNASSIGNED_REVIEW/LOOP_SSL_refresh_statistics.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/LOOP_SSL_refresh_statistics.csv` (git mv)
- `90_UNASSIGNED_REVIEW/LOOP_statistics_n10.csv` -> `04_RESULTS/E04_PRODUCTIVE_AL/LOOP_statistics_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/LOOP_statistics_n10.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/LOOP_statistics_n10.csv` (git blob copy)
- `90_UNASSIGNED_REVIEW/LOOP_summary.csv` -> `04_RESULTS/E04_PRODUCTIVE_AL/LOOP_summary.csv` (git mv)
- `90_UNASSIGNED_REVIEW/LOOP_summary.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/LOOP_summary.csv` (git blob copy)
- `90_UNASSIGNED_REVIEW/LOOP_T0_DAPT_same_AL_labels.csv` -> `04_RESULTS/E04_PRODUCTIVE_AL/LOOP_T0_DAPT_same_AL_labels.csv` (git mv)
- `90_UNASSIGNED_REVIEW/LOOP_T0_DAPT_same_AL_labels.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/LOOP_T0_DAPT_same_AL_labels.csv` (git blob copy)
- `90_UNASSIGNED_REVIEW/LOOP_T0_DAPT_same_AL_labels_statistics.csv` -> `04_RESULTS/E04_PRODUCTIVE_AL/LOOP_T0_DAPT_same_AL_labels_statistics.csv` (git mv)
- `90_UNASSIGNED_REVIEW/LOOP_T0_DAPT_same_AL_labels_statistics.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/LOOP_T0_DAPT_same_AL_labels_statistics.csv` (git blob copy)
- `90_UNASSIGNED_REVIEW/markdown(9).md eingefügt` -> `06_LOGS_AUDITS/markdown(9).md eingefügt` (git mv)
- `90_UNASSIGNED_REVIEW/MASTER_ap_equal_n_n10.csv` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/MASTER_ap_equal_n_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/MASTER_ap_n10.csv` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/MASTER_ap_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/MASTER_summary_n10.csv` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/MASTER_summary_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/MASTER_threshold_results_n10.csv` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/MASTER_threshold_results_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/N10_PROGRESS.json` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/N10_PROGRESS.json` (git mv)
- `90_UNASSIGNED_REVIEW/N10_RUN_NOTES.txt` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/N10_RUN_NOTES.txt` (git mv)
- `90_UNASSIGNED_REVIEW/phase5.log` -> `06_LOGS_AUDITS/phase5.log` (git mv)
- `90_UNASSIGNED_REVIEW/PRODUCTIVE_FINISH_ONLY_COMPLETE.json` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/PRODUCTIVE_FINISH_ONLY_COMPLETE.json` (git mv)
- `90_UNASSIGNED_REVIEW/PRODUCTIVE_FINISH_ONLY_COMPLETE.json` -> `06_LOGS_AUDITS/PRODUCTIVE_FINISH_ONLY_COMPLETE.json` (git blob copy)
- `90_UNASSIGNED_REVIEW/README_DO_NOT_USE_AS_FINAL_EVIDENCE.md` -> `99_LEGACY_PROVENANCE_ONLY/README_DO_NOT_USE_AS_FINAL_EVIDENCE.md` (git mv)
- `90_UNASSIGNED_REVIEW/README_INTERACTION.md` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/README_INTERACTION.md` (git mv)
- `90_UNASSIGNED_REVIEW/README_PENDING.md` -> `04_RESULTS/E07_REPLICATION10_PENDING/README_PENDING.md` (git mv)
- `90_UNASSIGNED_REVIEW/REQUIRED_REPRO_ASSETS.md` -> `05_REPRO_ASSETS_EXTERNAL/REQUIRED_REPRO_ASSETS.md` (git mv)
- `90_UNASSIGNED_REVIEW/rescued_b0_false_negatives_seed42.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/rescued_b0_false_negatives_seed42.csv` (git mv)
- `90_UNASSIGNED_REVIEW/results_long.csv` -> `04_RESULTS/E01_CORE_FREEZE/results_long.csv` (git mv)
- `90_UNASSIGNED_REVIEW/scenario_regression_audit.json` -> `04_RESULTS/E01_CORE_FREEZE/scenario_regression_audit.json` (git mv)
- `90_UNASSIGNED_REVIEW/scenario_regression_audit.json` -> `06_LOGS_AUDITS/scenario_regression_audit.json` (git blob copy)
- `90_UNASSIGNED_REVIEW/scenario_summary.csv` -> `04_RESULTS/E01_CORE_FREEZE/scenario_summary.csv` (git mv)
- `90_UNASSIGNED_REVIEW/shift_degradation.csv` -> `04_RESULTS/E01_CORE_FREEZE/shift_degradation.csv` (git mv)
- `90_UNASSIGNED_REVIEW/ssl_effects.csv` -> `04_RESULTS/E01_CORE_FREEZE/ssl_effects.csv` (git mv)
- `90_UNASSIGNED_REVIEW/STATISTICS_original5_replication5_pooled10.csv` -> `04_RESULTS/E03_FINAL_N10_PRIMARY/STATISTICS_original5_replication5_pooled10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/summary_metrics(2).csv` -> `04_RESULTS/E01_CORE_FREEZE/summary_metrics(2).csv` (git mv)
- `90_UNASSIGNED_REVIEW/system_25pct_results.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_25pct_results.csv` (git mv)
- `90_UNASSIGNED_REVIEW/system_25pct_summary.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_25pct_summary.csv` (git mv)
- `90_UNASSIGNED_REVIEW/system_ap_shift_corrected.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_ap_shift_corrected.csv` (git mv)
- `90_UNASSIGNED_REVIEW/T0_acquisition_audit.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/audit/T0_acquisition_audit.csv` (git mv)
- `90_UNASSIGNED_REVIEW/T0_ACTIVE_LEARNING_results_n10.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/T0_ACTIVE_LEARNING_results_n10.csv` (git mv)
- `90_UNASSIGNED_REVIEW/T0_E2E_training_history_seed42.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/T0_E2E_training_history_seed42.csv` (git mv)
- `90_UNASSIGNED_REVIEW/T0_E2E_training_history_seed52.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/T0_E2E_training_history_seed52.csv` (git mv)
- `90_UNASSIGNED_REVIEW/T0_E2E_training_history_seed62.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/T0_E2E_training_history_seed62.csv` (git mv)
- `90_UNASSIGNED_REVIEW/T0_E2E_training_history_seed72.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/T0_E2E_training_history_seed72.csv` (git mv)
- `90_UNASSIGNED_REVIEW/T0_E2E_training_history_seed82.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/T0_E2E_training_history_seed82.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE01_primary_interaction_25pct_fpr005.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/tables/TABLE01_primary_interaction_25pct_fpr005.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE01_SSL_refresh_primary.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/tables/TABLE01_SSL_refresh_primary.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE02_SSL_refresh_statistics.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/tables/TABLE02_SSL_refresh_statistics.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE02_stress_mean_25pct.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/tables/TABLE02_stress_mean_25pct.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE03_stress_mean_interaction_25pct.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/tables/TABLE03_stress_mean_interaction_25pct.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE03_T0_DAPT_same_AL_labels.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/tables/TABLE03_T0_DAPT_same_AL_labels.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE04_core_25pct_stress_mean.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/tables/TABLE04_core_25pct_stress_mean.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE04_T0_DAPT_same_AL_labels_statistics.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/tables/TABLE04_T0_DAPT_same_AL_labels_statistics.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE05_DAPT_T0_gap_random_vs_uncertainty.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/tables/TABLE05_DAPT_T0_gap_random_vs_uncertainty.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE05_productive_loop_summary.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/tables/TABLE05_productive_loop_summary.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE06_AL_gain_plot_data.csv` -> `04_RESULTS/E06_AL_SSL_ORIGINAL10/EXTRACTED/tables/TABLE06_AL_gain_plot_data.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE06_SSL_refresh_summary.csv` -> `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/tables/TABLE06_SSL_refresh_summary.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE_cascade_stress_all_fpr.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/TABLE_cascade_stress_all_fpr.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE_error_complementarity_stress.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/TABLE_error_complementarity_stress.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE_freeze_25pct_primary_fpr.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/TABLE_freeze_25pct_primary_fpr.csv` (git mv)
- `90_UNASSIGNED_REVIEW/TABLE_system_stress_all_fpr.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/TABLE_system_stress_all_fpr.csv` (git mv)
- `90_UNASSIGNED_REVIEW/testset_prevalence_audit.csv` -> `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/testset_prevalence_audit.csv` (git mv)

## Genuinely Unassigned Files
- None.

## Missing Manifest Paths By Class
### MISSING_BUT_PRESENT_INSIDE_EXISTING_ZIP
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed42_budget0p1.npz` SHA256=9096dd2458d5d1e294fb9e7cdb666f171c183f5196b5cd4c23eabecd0944d86b; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed42_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed42_budget0p25.npz` SHA256=bd93e30409f564279a9d9d1b9d6442bf2a08bd16ab08502db2529ce751d6e8b9; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed42_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed42_budget1p0.npz` SHA256=6f6fec45bf9d3d65cdceaa45eda2abfda0a67961a5ede18a6d1172bf6336c28b; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed42_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed52_budget0p1.npz` SHA256=82f41fafa49d6bc11ff284077eb7e7b9c14320ce0f2ff610e0ea06bb83f5c837; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed52_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed52_budget0p25.npz` SHA256=9c890a320f8d3ffc2ee996e4d9e1da9dfcb5711570775682151091fae3ca551d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed52_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed52_budget1p0.npz` SHA256=4faf7259a95a1d1715d58e2cdab3bba78e437dda042d258aa4508ffb8e7792af; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed52_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed62_budget0p1.npz` SHA256=84d89f3adc89ff0ed120a6df67b3c6996dba9f68008e6bd1725f51ee418ed6e0; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed62_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed62_budget0p25.npz` SHA256=f69a8ea53d8c9ed967ec06b9fb00e89b48c2e2d378771837650d08bd08d5df75; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed62_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed62_budget1p0.npz` SHA256=ab9af04ad9c9613c7d416c8f1eeddad9fec1476fe7e1f79f551372f916dfd444; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed62_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed72_budget0p1.npz` SHA256=5ac4df65bf551aa0c64b4392514e6d934dcc85a0f86545d3077bbcafb37b0fe6; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed72_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed72_budget0p25.npz` SHA256=185a5dc0b190d84607d7294da983516f0e2b3dc7aef0e7b572893ec93775ac06; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed72_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed72_budget1p0.npz` SHA256=94b62c4376b774ef0d2ef481c85b6f0ea666f0a6c4f2a9abb09dcfd58389cffe; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed72_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed82_budget0p1.npz` SHA256=d69569f27a35f1ea799291c920c9160a7354c90a8e6aab744bf6ddf0424b3bee; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed82_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed82_budget0p25.npz` SHA256=baf3c49ca5a985b6b81f00b8e6958041a44cb6d669ef373522ff9fc6bba205cd; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed82_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_LOGREG_seed82_budget1p0.npz` SHA256=9734a975441e9d70a8cc023ceb3236df5e14119f297e5e3ac9e2a04c8ff45d6c; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_LOGREG_seed82_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed42_budget0p1.npz` SHA256=bfbd2899012cc3c843ba18f93ecb703d63678283e4ac064851c6ab6ff63679be; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed42_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed42_budget0p25.npz` SHA256=5c1f6aa742a00f01556aeb0277cf1c303f5f88020383982cfeec9f72d73dcb05; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed42_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed42_budget1p0.npz` SHA256=12b1116790aab816ad0f3625e1b61c3d52967a1ebe046036e1cbe2ec895e05ae; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed42_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed52_budget0p1.npz` SHA256=244a16cecf8d61cf02bb70522f62328e45fe055eb08ae005266c991d69cce727; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed52_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed52_budget0p25.npz` SHA256=ea0226834a914668b0c27619bed67c369d24fe2f4e8f5aa9567bdb210589511a; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed52_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed52_budget1p0.npz` SHA256=6b7ba18c98baa449af75b0052f2242e7e1e53b38c56fc9a2aab6c6de1258aa9f; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed52_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed62_budget0p1.npz` SHA256=36bbfbd8db9f253afe9a39e6193013ce100772eac4b1edd40b77248bd41a7350; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed62_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed62_budget0p25.npz` SHA256=9169d030210750d0a214f07b77886415c4a47f82d57e6e3c3749eb0d83d5c6f1; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed62_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed62_budget1p0.npz` SHA256=b78469ac4af3c33193b14355993d6684b1fd427e5ab8b624a02acb2225a690d0; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed62_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed72_budget0p1.npz` SHA256=8d72be64d5d623b79a71270c2c2eff7cf0e5d2438c5aa8a81eea94450ef6b560; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed72_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed72_budget0p25.npz` SHA256=b5cc3b62933d62089c1f7d597339c2eb046c0dac4a8879bbbf52f17ef6d861da; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed72_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed72_budget1p0.npz` SHA256=33b05c9ff73a8145f3ab312c6d507e30ddba7476e710ac96e208c412ac90ac3c; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed72_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed82_budget0p1.npz` SHA256=98fde44f5c36ddf52973ef0875cea86b33965adea39f096f389e1357258bff9a; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed82_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed82_budget0p25.npz` SHA256=8724ca2e9eadf819e9888d60877270571fba4750b54e3d0598e6c387830cc77b; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed82_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_MLP_seed82_budget1p0.npz` SHA256=c10acc79507302663a6f36254e1a507dddf871f98ffd86ce7a289fae82c7a817; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_MLP_seed82_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed42_budget0p1.npz` SHA256=f7f5e93ba0e9d602bb1e92611f496a021a49c0b6124227f113c6216e1d536f97; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed42_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed42_budget0p25.npz` SHA256=4b3e8fd6e949157fdb639b2ed8ee5924a629011353666a4be081b2dfb5710a26; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed42_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed42_budget1p0.npz` SHA256=836a1ec0097dafa758883c0d5b1948da7cde8ccbcc2553d9883cdffd4886b322; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed42_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed52_budget0p1.npz` SHA256=9d80e6f6f7501a58674a0cab50d554f41bcbe7abeb48d06da09da372d6f7aa9a; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed52_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed52_budget0p25.npz` SHA256=223c72fef124d166dd09280ae1d42c6e706be89b1f3753321eeefd18e847212a; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed52_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed52_budget1p0.npz` SHA256=f3328b8c7b7c9ed1685405f3d19e92cfcbd021d25cca219318255e9af3cacf2d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed52_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed62_budget0p1.npz` SHA256=d9a1547ac1540019cdea2343d187fb86ae24d38e0cf6b91e0a6800c295c0bb5f; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed62_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed62_budget0p25.npz` SHA256=13dc612a0c8f98d66ef0fbfb4a4f1959a87883d128cecd6b526e95fa0c66250b; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed62_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed62_budget1p0.npz` SHA256=7e45718e2da8318f99df3dff6b4ce4170530dddef816cd4c290e379b33e3e27a; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed62_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed72_budget0p1.npz` SHA256=5b84a52c177c9f35a769003d5f52954e15e6b4aafe35e419e961302f11ae3892; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed72_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed72_budget0p25.npz` SHA256=d7630d1b04db31ec5cdbd6a07d6da7d119a4e71bda61afbbb4437437e7d85e93; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed72_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed72_budget1p0.npz` SHA256=c46110e0307aa275b56895945234b96fc10d37f45effaea742db5e3b8e2a2ed4; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed72_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed82_budget0p1.npz` SHA256=a2d78a55368e95fab04dd3664f141dfa321cdc2a4e3126c6ce5ac56ded5b7609; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed82_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed82_budget0p25.npz` SHA256=91d162a6bd9c6afc723342d304c87f0891ed52256bfeaf9ffc083be24223c8db; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed82_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/BASE_XGBOOST_seed82_budget1p0.npz` SHA256=710a0751caa2cc8cfce412d1aa964a2cd2620b3965f666e48e7abdbafb7b2ead; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/BASE_XGBOOST_seed82_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed42_budget0p1.npz` SHA256=a1f93d74767fec4b0b77eb08f51c6ddaeaa87c25db0e64094e65480fc3ddaf5d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed42_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed42_budget0p25.npz` SHA256=a9d436ac5542a25d4ef4e4a237ffa2d2f39caeb6522ca49b9c66f1100d9be338; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed42_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed42_budget1p0.npz` SHA256=0d34476a1de5debc583594f1354c7944439531e11fce311b3ca57665f71d1777; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed42_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed52_budget0p1.npz` SHA256=ed421b73aae71831476d336344dd707ba6b39e6198f64dfec3dbf9ccb2f8808a; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed52_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed52_budget0p25.npz` SHA256=616fbb31a6586162503bf537b48927578d0f5e70f50e0209dbe3f2342ad14d1d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed52_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed52_budget1p0.npz` SHA256=786393c3d2bf8700057404cc5aed6635726cef255691c4ba243e932fae081c53; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed52_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed62_budget0p1.npz` SHA256=e21de1599fcd4b817cc72d631c174738cf596bf623c8b6e3aa868ca094b73756; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed62_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed62_budget0p25.npz` SHA256=8ea95bf3f34d7599b258c3004f0c9c674d8599bfe10ff82a0bbb84c32743ca91; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed62_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed62_budget1p0.npz` SHA256=b5fd89164cffc0f5a5b98b8366f6c8c58c4b1ceeec3acf7d951920d9933c59fa; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed62_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed72_budget0p1.npz` SHA256=f828bd40ff65b687455ddba73c9310bd128bab95f086a41712cd687996c3a519; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed72_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed72_budget0p25.npz` SHA256=2aa0a628d02bdb15b489a1e6d738a35ed951fb85b26855e8203b41aed9b9e2b3; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed72_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed72_budget1p0.npz` SHA256=2b8c964714e43b7118bb0bf6650b437dd771ae98d6674a7924ac860612b997f9; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed72_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed82_budget0p1.npz` SHA256=7a7d8c69bf1f8a8f4bb57f6dc9b64fb03e3cad64160a8ce45433dab08cc929f5; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed82_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed82_budget0p25.npz` SHA256=a3673098bd926b4860db98ba58fee6ea6f8f4fe8fa967adbd7e119987184acd4; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed82_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_LOGREG_seed82_budget1p0.npz` SHA256=49e8773579a3904fa1f96c9301aebbab88a8930ab565b32f8b0b7c574cf6c3d7; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_LOGREG_seed82_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed42_budget0p1.npz` SHA256=d31c823b9d332aaa39a545f52d4813b02a2ab9d1b5233537983777dc7bf1d468; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed42_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed42_budget0p25.npz` SHA256=dd5c8582d31544cdda646ac4ea49a313e671196085f2567b2712d7e3344f9956; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed42_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed42_budget1p0.npz` SHA256=171a594786b276d28fa63caf17bf738d40125d4d0006b4ba3f8d359df55f76d3; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed42_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed52_budget0p1.npz` SHA256=ed6f50ea23873d485952390079cf9a9d97a107281d492ac547ace7d2027104f0; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed52_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed52_budget0p25.npz` SHA256=8566292f4323e29375ba3ff2b1432775863e7b5f24259af90b2333dc5bc32405; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed52_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed52_budget1p0.npz` SHA256=ea50ed308dcdbd0de792e10a3b91e3cfe593d272c8de508cf43d29a9125e0ac2; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed52_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed62_budget0p1.npz` SHA256=6547de6f7db20250d1247b71cdd762704a225556cc67713efa2d992d1bc03e1b; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed62_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed62_budget0p25.npz` SHA256=177085cc3437ce737fde6f671a1c1b89dc9b8a724ca9fe5843a5a43907d37ec3; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed62_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed62_budget1p0.npz` SHA256=8194f71e59327c54d0e2e88fb12ffd6b007d66e55f05d65b3895881efada11bb; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed62_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed72_budget0p1.npz` SHA256=d70bf9407311708fe50d0ace1eb0063c11e3f1222a38e8ce922e1240a61c853d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed72_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed72_budget0p25.npz` SHA256=b5e00c2fb563d236b4812937ff6055c075bd2974ebb0654fb42cfcb1808ff2d9; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed72_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed72_budget1p0.npz` SHA256=8570fbe311e0efedf294e23e6ac9a3a4f3d1ec93bce8723ecb9bc760e2d3378d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed72_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed82_budget0p1.npz` SHA256=7b976468b70a84e96b038a400b01f30e2f6fedb54b9298ea310c740909a8e489; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed82_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed82_budget0p25.npz` SHA256=82c4a2fbc350e0f5906ae9e9ba44d637890c65242b1c999a1ce0d161d786d202; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed82_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_MLP_seed82_budget1p0.npz` SHA256=55ff25c61f2d3cf674f5b1c4c9576493adb4b174ec477f01d436756f457ef879; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_MLP_seed82_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed42_budget0p1.npz` SHA256=068c93cedbd1676b9e541324c1ff667b3a1d5ba261f1d6fabe0a89dc102805fc; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed42_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed42_budget0p25.npz` SHA256=84a733879889f7d8c14c5b11a74f6607e1c2a77fdd97acdebf80b9d53dc7d5d1; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed42_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed42_budget1p0.npz` SHA256=570ecbe5a7894eed7833b31214948944df48cd9901f89331f379310281b6b2e8; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed42_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed52_budget0p1.npz` SHA256=9b08b9c37c0602c19b8ded75945dbb44fc82283e60f94c683aeec8719edd3438; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed52_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed52_budget0p25.npz` SHA256=d180f8b30528e7ef31c82d58c2d590bad1512c1584962a307722048599280adb; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed52_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed52_budget1p0.npz` SHA256=3e68a16f7ecd67c5c78544621b75544f868f8b7bc2f2a4ee01b5b4e9a84cadeb; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed52_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed62_budget0p1.npz` SHA256=c51552e39cba3a1eae3d34db8d88b49faef941d2d435117daeefc1ef7bb825d4; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed62_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed62_budget0p25.npz` SHA256=60d7fd493a700de399d0b7bbedb16aae30300a58c665d88629e6cf684bb33cb8; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed62_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed62_budget1p0.npz` SHA256=a8cccbb9b3d09661a1321b94ed99482953c0278a3134fecbeaf4a7c882417a1d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed62_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed72_budget0p1.npz` SHA256=70415ebf09ad42d2a05e8b292a4b94c47db57992492518621b32a35da9cae3e5; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed72_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed72_budget0p25.npz` SHA256=58bb85f2a472034cf4b248ecf6d0ce0e4d22260d5a51996493d65d79804ec1e2; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed72_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed72_budget1p0.npz` SHA256=f48c40ce79ab5651ef7e9debf85d14cd52388b4d967b636bf7c237c3ef3f0958; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed72_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed82_budget0p1.npz` SHA256=5f3fb68df7696bba10da5fc3a0465f3ee13a71bb2e684dc8f04c74b7fb9cfa7d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed82_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed82_budget0p25.npz` SHA256=645af8bc4f2739d466294decb70428ee39caa06af493f36a7260477ab7de65f7; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed82_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/CONTRASTIVE_XGBOOST_seed82_budget1p0.npz` SHA256=e18bfb7f63750d69077be3818f6761c24aa80b463687bbf4af21cf3fdb5f61e2; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/CONTRASTIVE_XGBOOST_seed82_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed42_budget0p1.npz` SHA256=ecbf0bdc7492fbde877ae7dfc4d92fdd344862386b4920bfd2307248141c1c72; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed42_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed42_budget0p25.npz` SHA256=8b1bc37d4b41f20f559d036913acd5169ab968cb0840228fc9b83f61e8380c22; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed42_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed42_budget1p0.npz` SHA256=9ffc74a734b99aafa95ca548218d82f15c69d6a10d17fe9370c29a8da4e29494; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed42_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed52_budget0p1.npz` SHA256=8083bb2eaa0a051bcfbfd3652366a840341ab7c0bd6d923469a4868363f9505e; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed52_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed52_budget0p25.npz` SHA256=0e09db36366c0fdd37508ba0a923d0203cd555a6bce7a35cedb6ac8a43001bf2; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed52_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed52_budget1p0.npz` SHA256=a139e071af651e80250a2977d51e1efd592d897bacf53f86be90e52f5d5f3769; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed52_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed62_budget0p1.npz` SHA256=4181afd6419936fd534e82acbf69485479cbb69c6b8f58b4343b38f7f7bc4a1c; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed62_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed62_budget0p25.npz` SHA256=2057deb7aafa38b45665dafd66fe3100465168bd553f162a563b857fa56662d3; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed62_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed62_budget1p0.npz` SHA256=1e07551a5bdfc5e7a3e840791f837d82d3aedfe1c5a7a069ccfb51d6def82f36; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed62_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed72_budget0p1.npz` SHA256=5f63ea9e9e988ae0371646cff2780ac494e9cffd2bf4a96ae558e780915c09eb; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed72_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed72_budget0p25.npz` SHA256=c910472a0e817539090c70abde9bcc49ab2f39b05a2ef7977beafa863c90a4e9; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed72_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed72_budget1p0.npz` SHA256=25dbd3ce5f91ac6b4e094e1343b78531d133f2349cbba15e96bd879734325440; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed72_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed82_budget0p1.npz` SHA256=ced0e92c4c9a76705cac6dde72659f81dc59c166bdd7465e11edb02ca066240b; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed82_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed82_budget0p25.npz` SHA256=4193cbecc94b9182dc25f8b55932ab1c9c53e519a754aac54731fe54850faa8f; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed82_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_LOGREG_seed82_budget1p0.npz` SHA256=4df8f3e57bf8fc6ff59070ba20e031753e8d8170985ea1b23484d72e40da794f; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_LOGREG_seed82_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed42_budget0p1.npz` SHA256=324923f485367c56739f361b9553b2e9d7b6fb233d60939e30ab66ff1d8b1335; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed42_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed42_budget0p25.npz` SHA256=b7c87c1ac7e353c3eb8ad1d4971cc778b309bd84e50a264dd42cac79c4ce5fd7; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed42_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed42_budget1p0.npz` SHA256=83a2f0458295e6bf7ef6abf655ad1128354d27217457cdccaa4f19a4121a728d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed42_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed52_budget0p1.npz` SHA256=3aba6f9ac043c335930a9c9541ee7513e51c820e7a464f38c494caf3ef5524b3; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed52_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed52_budget0p25.npz` SHA256=166da930cd743c1dbda558736f87facb72dcfefb38267623102ffc402c22dea6; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed52_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed52_budget1p0.npz` SHA256=e0bcf4290302f96c4744d2dac4c65af6327c4f7f60bf8c1c4aacf2b7b1f9b516; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed52_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed62_budget0p1.npz` SHA256=8e27aecfe0a3b703cd163fd8c08c074919aad7e84e6322ecef4b124cd1062afc; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed62_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed62_budget0p25.npz` SHA256=9c73475275ec4be0434dd83bfd6d97a09b60d36a12cbd8394e7ab67965e1c704; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed62_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed62_budget1p0.npz` SHA256=aff60808bdb08d39b8ce75cfa75c88aa1661e2da4f1dd44522c7fdab3b7aacd0; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed62_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed72_budget0p1.npz` SHA256=c6e22740948e930e6e044ed4fc39f229045aaa74b2882c88b8c982f22c7cf8e3; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed72_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed72_budget0p25.npz` SHA256=d559daec935e3f40c0e916a839417e1bb4b41aa40571a61f4412960203f01ec0; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed72_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed72_budget1p0.npz` SHA256=c9e69759f10927070054e59290b611b0364046c0d989946453a49e36703ba957; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed72_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed82_budget0p1.npz` SHA256=6b8af7f3bd3178008d4fde34b7029459c68bf14cfcdd1d9e09a7e35e314d7335; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed82_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed82_budget0p25.npz` SHA256=0eb470e65234d5f30c620b42e8b4789696a8ad35d89e56fd9e722f57f49fd14f; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed82_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_MLP_seed82_budget1p0.npz` SHA256=2fca99c9d9646144a91fb7ff9a7c241057f68242581f7052be22885cb679e3c5; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_MLP_seed82_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed42_budget0p1.npz` SHA256=98241a2fa63a6b660a11c51e9a35260003f1f334eaaa9bc359a75fe657622e2c; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed42_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed42_budget0p25.npz` SHA256=abe93a271ca7bd69dd04a10e989b4866baaa12292dedb242b0fac62db0c2d5fb; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed42_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed42_budget1p0.npz` SHA256=10f19d6c68f2818fdce41bc13620d5b08af6c73600a3c23124beafb37b3ffbad; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed42_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed52_budget0p1.npz` SHA256=9ccca093f80709d0556494a580b5d29e019fb2d4430fcd15e81f626c1b6fda69; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed52_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed52_budget0p25.npz` SHA256=404b050a858ea3f0eb49a18190f3a1f48e99f5a0a383fc040c08c4373327c1d0; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed52_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed52_budget1p0.npz` SHA256=3024211d1ddb846c05b3dcc2e992e715e8fbcc1af1fd248ed11e3db380ae6041; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed52_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed62_budget0p1.npz` SHA256=c23ad491e2606d302f2e87b50724d73be811fca8556771c377af2ba58225db1b; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed62_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed62_budget0p25.npz` SHA256=372e992feabd6b941faf0111be3f6b4fdbf683594beaf871fb954a0df6c0f245; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed62_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed62_budget1p0.npz` SHA256=5192e76c94244f5b4d63b38f67fea6491dc6aef65cf4ef103540076ed28fda4f; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed62_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed72_budget0p1.npz` SHA256=0438c9aec9cd20ffee582b7a2b64cd75911e21974e550549c028f8d028b8d670; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed72_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed72_budget0p25.npz` SHA256=dcf1277030f1f677e7e5c624cad0f4140c46add2e5e79657ef90517c0e54c2a4; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed72_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed72_budget1p0.npz` SHA256=ccb9bacc8384acfc39279c0f4143f23a00603d6205b813a2b71eb63d49599f3d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed72_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed82_budget0p1.npz` SHA256=34558317e46b0394c4e8355b83dccbb7a497be3114c48e23735ad4d415afebc9; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed82_budget0p1.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed82_budget0p25.npz` SHA256=4f1db763ae86a2a339c6502aed235c2910742d771175b1bc533b204b8143a2fa; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed82_budget0p25.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/freeze_scores/DAPT_XGBOOST_seed82_budget1p0.npz` SHA256=424582cf10bc0a189aeedc4c5655ea2b3059939bd25574c27d09f2f573e9337b; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::freeze_scores/DAPT_XGBOOST_seed82_budget1p0.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/B0_STRUCT_XGB_seed42.npz` SHA256=f7b9ffd6a9dcff5e6def4526c1f3789ab241e674a6abe746a31423601171cc41; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/B0_STRUCT_XGB_seed42.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/B0_STRUCT_XGB_seed52.npz` SHA256=423c4b4bf11c4b9611c60250882da3cb05bf58dd87e678c59ceced4c9d5f5053; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/B0_STRUCT_XGB_seed52.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/B0_STRUCT_XGB_seed62.npz` SHA256=347a5cfbc5892687975719506f4fbdc3c09ce97428a966c2c427f8bdb7fc738b; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/B0_STRUCT_XGB_seed62.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/B0_STRUCT_XGB_seed72.npz` SHA256=f7a3551924a837b49840f9daca0eb83b0fbbc056204d4ffb45e263ac7359a0b5; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/B0_STRUCT_XGB_seed72.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/B0_STRUCT_XGB_seed82.npz` SHA256=0bcdf655d58eaa6b1c6e59e6da59fd8de8af520f978a07da2761ae9b2e0082f6; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/B0_STRUCT_XGB_seed82.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/BASE_EMB_MLP_seed42.npz` SHA256=5c1f6aa742a00f01556aeb0277cf1c303f5f88020383982cfeec9f72d73dcb05; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/BASE_EMB_MLP_seed42.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/BASE_EMB_MLP_seed52.npz` SHA256=ea0226834a914668b0c27619bed67c369d24fe2f4e8f5aa9567bdb210589511a; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/BASE_EMB_MLP_seed52.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/BASE_EMB_MLP_seed62.npz` SHA256=9169d030210750d0a214f07b77886415c4a47f82d57e6e3c3749eb0d83d5c6f1; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/BASE_EMB_MLP_seed62.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/BASE_EMB_MLP_seed72.npz` SHA256=b5cc3b62933d62089c1f7d597339c2eb046c0dac4a8879bbbf52f17ef6d861da; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/BASE_EMB_MLP_seed72.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/BASE_EMB_MLP_seed82.npz` SHA256=8724ca2e9eadf819e9888d60877270571fba4750b54e3d0598e6c387830cc77b; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/BASE_EMB_MLP_seed82.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/CONTRASTIVE_EMB_MLP_seed42.npz` SHA256=dd5c8582d31544cdda646ac4ea49a313e671196085f2567b2712d7e3344f9956; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/CONTRASTIVE_EMB_MLP_seed42.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/CONTRASTIVE_EMB_MLP_seed52.npz` SHA256=8566292f4323e29375ba3ff2b1432775863e7b5f24259af90b2333dc5bc32405; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/CONTRASTIVE_EMB_MLP_seed52.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/CONTRASTIVE_EMB_MLP_seed62.npz` SHA256=177085cc3437ce737fde6f671a1c1b89dc9b8a724ca9fe5843a5a43907d37ec3; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/CONTRASTIVE_EMB_MLP_seed62.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/CONTRASTIVE_EMB_MLP_seed72.npz` SHA256=b5e00c2fb563d236b4812937ff6055c075bd2974ebb0654fb42cfcb1808ff2d9; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/CONTRASTIVE_EMB_MLP_seed72.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/CONTRASTIVE_EMB_MLP_seed82.npz` SHA256=82c4a2fbc350e0f5906ae9e9ba44d637890c65242b1c999a1ce0d161d786d202; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/CONTRASTIVE_EMB_MLP_seed82.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/DAPT_E2E_seed42.npz` SHA256=dbd8a2a6bf4be39fd5877ea784d6bbe5737e28627dd561693cecaaad0dca6de8; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/DAPT_E2E_seed42.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/DAPT_E2E_seed52.npz` SHA256=1c4d87f4528132b3cf2400b97341027e371c475985acea162fa6262c9f05c42e; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/DAPT_E2E_seed52.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/DAPT_E2E_seed62.npz` SHA256=37ff35cb9097d2cab30b6d1545ad6de9efa89d80e1d6c08941808b7c7fc87d61; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/DAPT_E2E_seed62.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/DAPT_E2E_seed72.npz` SHA256=afdcc644abfc00587c8b32d3cc075652780bfcbaea41db48fa1656aadb75cbb4; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/DAPT_E2E_seed72.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/DAPT_E2E_seed82.npz` SHA256=054edd09abd43f452a2c83bdbd47af606ce09a19a0b56aebd3ac8180f7c6c6b5; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/DAPT_E2E_seed82.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/DAPT_EMB_MLP_seed42.npz` SHA256=b7c87c1ac7e353c3eb8ad1d4971cc778b309bd84e50a264dd42cac79c4ce5fd7; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/DAPT_EMB_MLP_seed42.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/DAPT_EMB_MLP_seed52.npz` SHA256=166da930cd743c1dbda558736f87facb72dcfefb38267623102ffc402c22dea6; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/DAPT_EMB_MLP_seed52.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/DAPT_EMB_MLP_seed62.npz` SHA256=9c73475275ec4be0434dd83bfd6d97a09b60d36a12cbd8394e7ab67965e1c704; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/DAPT_EMB_MLP_seed62.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/DAPT_EMB_MLP_seed72.npz` SHA256=d559daec935e3f40c0e916a839417e1bb4b41aa40571a61f4412960203f01ec0; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/DAPT_EMB_MLP_seed72.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/DAPT_EMB_MLP_seed82.npz` SHA256=0eb470e65234d5f30c620b42e8b4789696a8ad35d89e56fd9e722f57f49fd14f; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/DAPT_EMB_MLP_seed82.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/T0_E2E_seed42.npz` SHA256=de365a616059ea815e33b709f201e5d0c41d69df4af7f9309bad2619b15d9c7d; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/T0_E2E_seed42.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/T0_E2E_seed52.npz` SHA256=b64c92c95e86949b90e6d6caa80ad0b91e632c2b292588830a4a8acd4031f07e; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/T0_E2E_seed52.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/T0_E2E_seed62.npz` SHA256=27119a8458e0cfbfd3ce79294eda6f61a901b97fd70a7346af3b605f01c852b6; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/T0_E2E_seed62.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/T0_E2E_seed72.npz` SHA256=2734d06af35e79d6384c710b9f9661ead89abc470c902132583c86cc3bcc3a1a; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/T0_E2E_seed72.npz`
- `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/EXTRACTED/system_scores/T0_E2E_seed82.npz` SHA256=d9c60993fb2a4fceb41a51356eecd1fe307691b9d8d73f040046bad5cdf81d6f; zip evidence: `04_RESULTS/E02_HYBRID_5SEED_SUPPORT/phreshphish_hybrid_freeze_extension.zip::system_scores/T0_E2E_seed82.npz`
### INTENTIONAL_EXTERNAL_REPRO_ASSET
- None.
### MISSING_AND_NOT_PRESENT_IN_REPOSITORY
- `04_RESULTS/E05_SSL_REFRESH_ABLATION/EXTRACTED/audit/FINISH_PROGRESS.json` SHA256=451c6303212c4886ff25ed337016301876604bc7a4e0a13fb668a7472f96161e
- `04_RESULTS/E05_SSL_REFRESH_ABLATION/phreshphish_PRODUCTIVE_LOOP_FINISH_ONLY_ANALYSIS.zip` SHA256=ddcf2f06fdc86aff3b021af62ad5b632bd969519050aa3ca7f0c530e44328928

## Mismatched Existing Manifest Paths
- None.

## External Reproducibility Assets Still Required
- R1 TokenCache / final freeze tokens, embeddings, contrastive encoders, and full freeze output.
- R2 RoBERTa-base model artifact.
- R3 ENDGAME full assets, including DAPT40k bundle/splits and original encoder state where available.
- R4 complete FINAL-N10 Kaggle output with all tables, figures, encoders, score caches, and audits.
- R5 complete productive loop `lpppll` state cache including `state_scores/*.npz`.
- R6 ALxSSL Original10 full state cache if available.
- R7 Replication10 full output after completion.

## git diff --stat HEAD
```
00_START_HERE/CURRENT_FILE_INVENTORY.csv           |  209 +-
 .../E01_CORE_FREEZE}/FINAL_FREEZE_COMPLETE.json    |    0
 .../E01_CORE_FREEZE}/artifact_audit.json           |    0
 .../E01_CORE_FREEZE}/best_classifier_params.json   |    0
 .../E01_CORE_FREEZE}/classifier_tuning.csv         |    0
 .../E01_CORE_FREEZE}/configuration.json            |    0
 .../contrastive_training_history.csv               |    0
 .../effect_confidence_intervals.csv                |    0
 .../E01_CORE_FREEZE}/label_budget_audit.csv        |    0
 .../E01_CORE_FREEZE}/results_long.csv              |    0
 .../scenario_regression_audit.json                 |    0
 .../E01_CORE_FREEZE}/scenario_summary.csv          |    0
 .../E01_CORE_FREEZE}/shift_degradation.csv         |    0
 .../E01_CORE_FREEZE}/ssl_effects.csv               |    0
 .../E01_CORE_FREEZE}/summary_metrics(2).csv        |    0
 .../DAPT_E2E_training_history_seed42.csv           |    0
 .../DAPT_E2E_training_history_seed52.csv           |    0
 .../DAPT_E2E_training_history_seed62.csv           |    0
 .../DAPT_E2E_training_history_seed72.csv           |    0
 .../DAPT_E2E_training_history_seed82.csv           |    0
 .../HYBRID_FREEZE_EXTENSION_COMPLETE.json          |    0
 .../EXTRACTED}/T0_E2E_training_history_seed42.csv  |    0
 .../EXTRACTED}/T0_E2E_training_history_seed52.csv  |    0
 .../EXTRACTED}/T0_E2E_training_history_seed62.csv  |    0
 .../EXTRACTED}/T0_E2E_training_history_seed72.csv  |    0
 .../EXTRACTED}/T0_E2E_training_history_seed82.csv  |    0
 .../EXTRACTED}/TABLE_cascade_stress_all_fpr.csv    |    0
 .../TABLE_error_complementarity_stress.csv         |    0
 .../EXTRACTED}/TABLE_freeze_25pct_primary_fpr.csv  |    0
 .../EXTRACTED}/TABLE_system_stress_all_fpr.csv     |    0
 .../EXTRACTED}/ap_equal_n_sensitivity_results.csv  |    0
 .../ap_shift_corrected_prevalence_matched.csv      |    0
 .../EXTRACTED}/ap_shift_equal_n_sensitivity.csv    |    0
 .../EXTRACTED}/b0_structural_feature_columns.csv   |    0
 .../EXTRACTED}/b0_train_only_tuning.csv            |    0
 .../EXTRACTED}/cascade_results.csv                 |    0
 .../EXTRACTED}/cascade_summary.csv                 |    0
 .../EXTRACTED}/error_complementarity.csv           |    0
 .../EXTRACTED}/error_complementarity_summary.csv   |    0
 .../EXTRACTED}/error_feature_profiles_seed42.csv   |    0
 .../EXTRACTED}/freeze_corrected_results.csv        |    0
 .../EXTRACTED}/freeze_corrected_summary.csv        |    0
 .../EXTRACTED/label_budget_audit.csv               |   16 +
 .../rescued_b0_false_negatives_seed42.csv          |    0
 .../EXTRACTED}/system_25pct_results.csv            |    0
 .../EXTRACTED}/system_25pct_summary.csv            |    0
 .../EXTRACTED}/system_ap_shift_corrected.csv       |    0
 .../EXTRACTED}/testset_prevalence_audit.csv        |    0
 .../ACTIVE_LEARNING_full_matrix_n10.csv            |    0
 .../ACTIVE_LEARNING_summary_n10.csv                |    0
 .../CASCADE_STAGE1_JUSTIFICATION.csv               |    0
 .../CASCADE_stage1_sensitivity_n10.csv             |    0
 .../CASCADE_stage1_sensitivity_summary_n10.csv     |    0
 .../E03_FINAL_N10_PRIMARY}/FINAL_N10_COMPLETE.json |    0
 .../MASTER_ap_equal_n_n10.csv                      |    0
 .../E03_FINAL_N10_PRIMARY}/MASTER_ap_n10.csv       |    0
 .../E03_FINAL_N10_PRIMARY}/MASTER_summary_n10.csv  |    0
 .../MASTER_threshold_results_n10.csv               |    0
 .../E03_FINAL_N10_PRIMARY}/N10_PROGRESS.json       |    0
 .../E03_FINAL_N10_PRIMARY}/N10_RUN_NOTES.txt       |    0
 .../STATISTICS_original5_replication5_pooled10.csv |    0
 .../LOOP_T0_DAPT_same_AL_labels.csv                |    0
 .../LOOP_T0_DAPT_same_AL_labels_statistics.csv     |    0
 .../E04_PRODUCTIVE_AL}/LOOP_acquisition_audit.csv  |    0
 .../LOOP_annotation_efficiency.csv                 |    0
 .../E04_PRODUCTIVE_AL}/LOOP_results_long.csv       |    0
 .../E04_PRODUCTIVE_AL}/LOOP_statistics_n10.csv     |    0
 .../E04_PRODUCTIVE_AL}/LOOP_summary.csv            |    0
 .../EXTRACTED}/LOOP_SSL_refresh_ablation.csv       |    0
 .../EXTRACTED}/LOOP_SSL_refresh_statistics.csv     |    0
 .../EXTRACTED/LOOP_T0_DAPT_same_AL_labels.csv      | 1081 ++++
 .../LOOP_T0_DAPT_same_AL_labels_statistics.csv     |   21 +
 .../EXTRACTED/LOOP_acquisition_audit.csv           |   91 +
 .../EXTRACTED/LOOP_annotation_efficiency.csv       |   13 +
 .../EXTRACTED/LOOP_results_long.csv                | 6481 ++++++++++++++++++++
 .../EXTRACTED/LOOP_statistics_n10.csv              |   33 +
 .../EXTRACTED/LOOP_summary.csv                     |  649 ++
 .../PRODUCTIVE_FINISH_ONLY_COMPLETE.json           |    0
 .../EXTRACTED/figures}/figure_manifest.csv         |    0
 .../tables}/TABLE01_SSL_refresh_primary.csv        |    0
 .../tables}/TABLE02_SSL_refresh_statistics.csv     |    0
 .../tables}/TABLE03_T0_DAPT_same_AL_labels.csv     |    0
 .../TABLE04_T0_DAPT_same_AL_labels_statistics.csv  |    0
 .../tables}/TABLE05_productive_loop_summary.csv    |    0
 .../tables}/TABLE06_SSL_refresh_summary.csv        |    0
 .../EXTRACTED}/AL_SSL_INTERACTION_COMPLETE.json    |    0
 .../EXTRACTED}/AL_SSL_INTERACTION_results_long.csv |    0
 .../AL_SSL_INTERACTION_statistics_n10.csv          |    0
 .../EXTRACTED}/DAPT_T0_gaps_by_AL_strategy.csv     |    0
 .../EXTRACTED}/README_INTERACTION.md               |    0
 .../EXTRACTED}/T0_ACTIVE_LEARNING_results_n10.csv  |    0
 .../audit}/AL_SSL_INTERACTION_PROGRESS.json        |    0
 .../EXTRACTED/audit}/T0_acquisition_audit.csv      |    0
 .../TABLE01_primary_interaction_25pct_fpr005.csv   |    0
 .../tables}/TABLE02_stress_mean_25pct.csv          |    0
 .../TABLE03_stress_mean_interaction_25pct.csv      |    0
 .../tables}/TABLE04_core_25pct_stress_mean.csv     |    0
 .../TABLE05_DAPT_T0_gap_random_vs_uncertainty.csv  |    0
 .../tables}/TABLE06_AL_gain_plot_data.csv          |    0
 .../E07_REPLICATION10_PENDING}/README_PENDING.md   |    0
 .../REQUIRED_REPRO_ASSETS.md                       |    0
 06_LOGS_AUDITS/AL_SSL_INTERACTION_COMPLETE.json    |   74 +
 06_LOGS_AUDITS/FINAL_FREEZE_COMPLETE.json          |    8 +
 06_LOGS_AUDITS/FINAL_N10_COMPLETE.json             |   88 +
 .../HYBRID_FREEZE_EXTENSION_COMPLETE.json          |   51 +
 .../PRODUCTIVE_FINISH_ONLY_COMPLETE.json           |   39 +
 06_LOGS_AUDITS/artifact_audit.json                 |   12 +
 .../markdown(9).md eingef\303\274gt"               |    0
 .../phase5.log                                     |    0
 06_LOGS_AUDITS/scenario_regression_audit.json      |   42 +
 .../README_DO_NOT_USE_AS_FINAL_EVIDENCE.md         |    0
 111 files changed, 8812 insertions(+), 96 deletions(-)
```
