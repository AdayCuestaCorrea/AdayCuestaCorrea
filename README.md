# Aday Cuesta Correa

Junior Data Engineer / Data Scientist based in Tenerife, Spain. Computer Engineer (Universidad de La Laguna) and MSc in Big Data and Data Science (VIU, 2026).

## Featured projects

**[Paleo Atlas](https://github.com/AdayCuestaCorrea/paleo-atlas)** · [website](https://adaycuestacorrea.github.io/paleo-atlas/)
A bilingual (ES/EN) paleontology encyclopedia that rebuilds itself every day from 9 open scientific sources, at no cost.
- Raw responses versioned in git → dbt + DuckDB (66 models, SCD type 2 history) → static site on GitHub Pages, run daily by GitHub Actions and, with the same commands, by Airflow DAGs.
- 932,494 GBIF fossil specimens reconciled with PBDB in DuckDB and PySpark, with a [benchmark](https://github.com/AdayCuestaCorrea/paleo-atlas/blob/main/benchmarks/gbif/results.md) behind the choice of engine.
- LLM-written pages where every sentence cites a sourced fact and passes automatic checks; LLM news classification measured against hand labels.
- 302 pytest and 196 dbt tests on every run.

**[Daily public transport demand in Madrid](https://github.com/AdayCuestaCorrea/TFM)** · MSc thesis (8/10)
1,310 days of data and 161 features; 11 models compared, from baselines to SARIMAX, XGBoost, LSTM and a residual LSTM-XGBoost hybrid. The best, a SARIMAX + XGBoost ensemble, reaches 3.1 % MAPE and R² 0.976 on 197 test days, against 7.2 % for the seasonal baseline, with walk-forward validation and no leakage.

## Tools

Python · SQL · dbt · DuckDB · Airflow · PySpark · GitHub Actions · Docker · pandas · scikit-learn · XGBoost · TensorFlow/Keras · LLMs (Ollama, Groq)

## Contact

[LinkedIn](https://www.linkedin.com/in/aday-cuesta-correa-b26636272)
