# Lightweight Evidence

Use the executed notebook outputs for screenshots. Key passing metrics from this run:

- NB1: schema enforcement blocked `age=str`; `schema_mode="merge"` added `tier`.
- NB2: files before optimize `200`; files after `55`; speedup `10.0x`; files-pruned ratio `55.0x`.
- NB3: MERGE 100K rows `0.05s`; RESTORE `0.01s`; `score < 0` count after restore `0`; total versions `5`.
- NB4: Bronze `200,000`; Silver `190,052`; duplicates dropped `9,948`; Gold dates `8`; models `3`; rows `24`.

Local Delta logs exist under `_lakehouse/*/*/_delta_log/`, including:

- `_lakehouse/scratch/users_delta/_delta_log/00000000000000000000.json`
- `_lakehouse/scratch/events_smallfiles/_delta_log/00000000000000000000.json`
- `_lakehouse/scratch/customers_tt/_delta_log/00000000000000000004.json`
- `_lakehouse/bronze/llm_calls_raw/_delta_log/00000000000000000000.json`
- `_lakehouse/silver/llm_calls/_delta_log/00000000000000000000.json`
- `_lakehouse/gold/llm_daily_metrics/_delta_log/00000000000000000001.json`
