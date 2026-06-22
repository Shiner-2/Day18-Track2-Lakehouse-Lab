# Submission Checklist

**MSV:** 2A202600629  
**Ho va ten:** Pham Ngoc Hai Duong

- [x] NB1 executed: Delta table, `_delta_log`, schema enforcement, schema evolution `tier`.
- [x] NB2 executed: small files >= 100, OPTIMIZE+ZORDER, speedup/pruned ratio pass.
- [x] NB3 executed: MERGE 100K, RESTORE, history >= 5 versions.
- [x] NB4 executed: Bronze/Silver/Gold, Silver < Bronze, Gold >= 7 dates x 3 models.
- [x] Screenshots saved in `submission/screenshots/`.
- [x] Reflection written in `submission/REFLECTION.md` under 200 words.
- [x] Executed `.ipynb` notebooks included with outputs preserved.
- [x] `_lakehouse/` not committed.
- [x] `.venv/` not committed.

## Files to Commit

- `.gitignore`
- `notebooks/01_delta_basics.ipynb`
- `notebooks/02_optimize_zorder.ipynb`
- `notebooks/03_time_travel.ipynb`
- `notebooks/04_medallion.ipynb`
- `submission/REFLECTION.md`
- `submission/CHECKLIST.md`
- `submission/screenshots/*`

## Push Target

```text
origin/main
```
