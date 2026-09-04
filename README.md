# Machine Unlearning: Loss Granularity in a GPT-like Language Model

This repository contains the experimental notebooks and benchmark artifacts
used for a bachelor thesis on Gradient-Ascent-based machine unlearning in a
self-trained GPT-like language model.

The experiments compare sequence-wide and token-selective forget losses on the
controlled factual relation `capital(Pakistan, Islamabad)`. The repository
includes baseline pretraining, corpus and candidate search, pre-evaluation,
Gradient-Ascent unlearning, reference-model training, and the final result
analysis.

## Notebooks

1. `baseline_pretraining_M0.ipynb` – pretraining of the baseline model `M0`
2. `corpus_candidate_search_pakistan_islamabad.ipynb` – corpus search and export of candidate evidence windows
3. `pre_evaluation_M0_final_benchmark.ipynb` – baseline evaluation on the frozen benchmark
4. `gradient_ascent_unlearning_final_logging_clean.ipynb` – Full-Window and token-selective Gradient Ascent runs
5. `reference_model_training_Mref.ipynb` – construction of the modified corpus and training of `M_ref`
6. `thesis_results_analysis_clean.ipynb` – aggregation, comparison, full validation, matched-forgetting analysis, and thesis figures

The final classification of candidate evidence windows was performed manually.
Large model checkpoints and cached token tensors are not included in the repository.
