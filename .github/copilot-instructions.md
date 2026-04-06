Project: Telco Customer Churn — Data Analysis

Guidelines for assistant collaborators / Copilot:

- Notebook language: Spanish. The main deliverable is `notebooks/analysis-es.ipynb` and all narrative, headings and explanations inside that notebook must be written in Spanish.
- All files outside the notebook (README, docs, code, instructions) must be in English.
- Do not touch the data/ directory.
- Data source: Kaggle dataset `abdallahwagih/telco-customer-churn`. Use the Kaggle API programmatically (the `kaggle` Python package) to fetch files at runtime. Require the user to provide credentials via `~/.kaggle/kaggle.json` or environment variables. Do not commit credentials to the repo.
- Keep the README concise — a short project summary, quick start, and license line is enough.
- Cleanup performed: removed placeholder `.gitkeep` files from `data/raw`, `data/processed`, and `output/figures`.
- Do not remove or modify `src/utils.py` or `docs/project-summary.md` unless explicitly requested.
- When editing the notebook, keep changes minimal and focused: imports first, then data-loading, then EDA, visualization, conclusions in separate small cells.
- When presenting notebook content in chat, show cells in VS Code XML cell format and reference cells by number (1-based). Do not expose internal cell IDs.

If you need to fetch the Kaggle dataset in the notebook, use `KaggleApi` and `dataset_download_files(..., unzip=True)` then `pd.read_csv()` on the downloaded CSV.
