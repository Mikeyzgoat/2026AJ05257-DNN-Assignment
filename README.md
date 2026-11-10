# DNN Assignment 2

Student: T ADITYA ANANDA SAI
BITS ID: 2026AJ05257

The two notebooks are self-contained and follow the supplied assignment PDF. They use Python 3.10+, PyTorch 2.x, NumPy, pandas, Matplotlib, scikit-learn and `ucimlrepo`. UCI HAR is downloaded and cached when its notebook cell is run; Tiny Shakespeare is downloaded by the Problem 2 notebook.

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Run `problem1/problem1.ipynb` and `problem2/problem2.ipynb` from top to bottom. Each notebook contains its own imports, data pipeline, checks, experiment helpers and plotting code. Results are appended to `results.csv`, and figures are written under the relevant `figures/` folder.

The student-specific odd-ID ablation is LSTM forget-gate bias 0 versus 1 at `T=200`. The custom recurrent cells, restricted attention, Transformer, training helpers, sampling, heatmaps, and profiling code are implemented. Long-running data downloads and experiments remain opt-in via the notebook flags/comments, so no fabricated results are committed.
