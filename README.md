# LSH–BRB experiment

This experiment compares exact local rule matching with p-stable LSH candidate
retrieval under identical stratified folds. It reuses the dataset loaders and
train-only preprocessing from `/Users/lin/Documents/vfl+brb+dis`.

Run a smoke test:

```bash
python3 experiments/run_lsh_brb.py --datasets breast_cancer --folds 2 \
  --output results/lsh_brb_smoke
```

Run the six manuscript datasets:

```bash
python3 experiments/run_lsh_brb.py \
  --datasets spect_heart heart_disease diabetes cdc_diabetes_multiclass \
             breast_cancer_recurrence new_thyroid \
  --folds 5 --seed 13 --top-q 25 --output results/lsh_brb_six_datasets
```
