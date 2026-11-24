# Aday Cuesta Correa

Junior Data Engineer / Data Scientist based in Tenerife, Spain. Computer Engineer (Universidad de La Laguna) and MSc in Big Data and Data Science (VIU, 2026).

## Featured projects

**[Paleo Atlas](https://github.com/AdayCuestaCorrea/paleo-atlas)** · [website](https://adaycuestacorrea.github.io/paleo-atlas/)
A bilingual (ES/EN) paleontology encyclopedia that rebuilds itself every day from 9 open scientific sources, at no cost.
- Raw responses versioned in git → dbt + DuckDB (66 models, SCD type 2 history) → static site on GitHub Pages, run daily by GitHub Actions and, with the same commands, by Airflow DAGs.
- 932,494 GBIF fossil specimens reconciled with PBDB in DuckDB and PySpark, with a [benchmark](https://github.com/AdayCuestaCorrea/paleo-atlas/blob/main/benchmarks/gbif/results.md) behind the choice of engine.
- LLM-written pages where every sentence cites a sourced fact and passes automatic checks; LLM news classification measured against hand labels.
- 302 pytest and 196 dbt tests on every run.

**[AI agent team](https://github.com/AdayCuestaCorrea/equipo-agentes-ia)** · [demo](https://agentes-ia-aday.vercel.app/)
Three agents (Orchestrator, Develop and Testing) that modify a sample HTML/CSS website, with a live preview of every version.
- The Orchestrator splits a request into tasks with typed acceptance criteria; Develop delivers complete files, and each delivery is a new version.
- Testing combines deterministic checks (well-formed HTML, title and lang, links, labelled form fields) with an LLM review, and sends failures back to Develop, up to 3 attempts per task.
- Structured JSON output validated with zod, with a fallback between LLM providers (Groq and Gemini), logged with provider, model and latency.
- One agent step per invocation on Vercel, with state and an atomic lease in Postgres (Supabase). 84 Vitest tests. Built with Claude Code.

**[Synaptica](https://github.com/AdayCuestaCorrea/synaptica)** · [website](https://adaycuestacorrea.github.io/synaptica/es/index.html) · *in development, with a neuroscience PhD student (scientific review)*
A bilingual (ES/EN) neuroscience hub that updates itself every day from open sources, at no cost. Built on the Paleo Atlas engine.
- Daily GitHub Actions pipeline: PubMed, Europe PMC, bioRxiv/medRxiv, Crossref retractions, OpenAlex and journal feeds → dbt + DuckDB warehouse with tests → static site, mirrored weekly to BigQuery.
- LLM summaries (Groq) where every sentence cites its facts, numbers and names must match the source, and a judge model of another family must pass them; anything that fails falls back to data-only text.
- Human in the loop: the neuroscientist approves, corrects or rejects a sample of summaries from the browser, and those decisions come back as GitHub Issues that are applied automatically.
- Interactive 3D brain models to explore, the first piece of the upcoming Neuro Atlas.

**[Daily public transport demand in Madrid](https://github.com/AdayCuestaCorrea/TFM)** · MSc thesis (8/10)
1,310 days of data and 161 features; 11 models compared, from baselines to SARIMAX, XGBoost, LSTM and a residual LSTM-XGBoost hybrid. The best, a SARIMAX + XGBoost ensemble, reaches 3.1 % MAPE and R² 0.976 on 197 test days, against 7.2 % for the seasonal baseline, with walk-forward validation and no leakage.

## Tools

Python · SQL · TypeScript · Next.js · dbt · DuckDB · Airflow · PySpark · BigQuery · GitHub Actions · Docker · Postgres (Supabase) · pandas · scikit-learn · XGBoost · TensorFlow/Keras · LangChain/LangGraph · LLMs (OpenAI, Groq, Gemini, Ollama)

## Contact

[LinkedIn](https://www.linkedin.com/in/aday-cuesta-correa-b26636272)
