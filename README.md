Reference paper: [MIMIC-IV-ED Benchmark](https://www.nature.com/articles/s41597-022-01782-9)<br/>
Forked from: [nliulab/mimic4ed-benchmark](https://github.com/nliulab/mimic4ed-benchmark)

=========================
## Instructions

1. Update data directory paths in `dataset_path.py`.
2. Preprocess the data by running the following Jupyter notebooks in `Benchmark_scripts`:
    1. `extract_master_dataset.ipynb`: Generates `data/master_dataset.csv` which includes all relevant patient information
    2. `data_general_processing.ipynb`: Generates `data/train.csv` and `data/test.csv` for model training and testing
3. Perform model training and testing by running the following Jupyter notebooks in `Benchmark_scripts`:
    1. `Task_1_Model_hospitalization_triage.ipynb`: Predicting hospitalisation at triage
    2. `Task_2_Model_critical_triage.ipynb`: Predicting critical outcomes at triage
    3. `Task_3_Model_72h_ed_revisit_disposition.ipynb`: Predicting ED revisit within 72 hours at disposition
    4. `Task_4_Model_triage_arrival.ipynb`: Predicting triage level at arrival
4. Analyse the results by running
    `Benchmark_scripts/plot_results.ipynb`
