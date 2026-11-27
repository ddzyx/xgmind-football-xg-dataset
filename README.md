# XG Mind — Open Historical Football Match & xG Dataset

[![Harvard Dataverse DOI](https://img.shields.io/badge/DOI-10.7910%2FDVN%2FIJ84J8-1e40af)](https://doi.org/10.7910/DVN/IJ84J8)
[![Terminal](https://img.shields.io/badge/XG%20Mind-xgmind.com-10b981)](https://xgmind.com/)
[![Public Ledger](https://img.shields.io/badge/Open%20Ledger-Verified-blue)](https://xgmind.com/performance/)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

> *Compiled from publicly available sports statistics and processed by XG Mind Data Engine ([https://xgmind.com](https://xgmind.com/)).*

Weekly updated, normalized historical match statistics and expected goals (xG) benchmark covering **completed** fixtures across major European competitions (Premier League, La Liga, Serie A, Bundesliga, Ligue 1, UEFA Champions League, Europa League, and top domestic leagues).

- **Dataset Size**: **4,000 completed fixtures** (**3,811 matches** with non-null `xg_home` / `xg_away`)
- **Last Automated Sync**: 2026-11-27 12:26 UTC
- **Formats**: CSV (`data/european_football_xg_matches.csv`) + Parquet (`data/european_football_xg_matches.parquet`)
- **Academic Citation (Harvard Dataverse)**: [10.7910/DVN/IJ84J8](https://doi.org/10.7910/DVN/IJ84J8) ([Harvard Dataverse Landing Page](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/IJ84J8))

## Column Schema

| Column | Description |
| :--- | :--- |
| `match_id`, `match_date`, `season_year`, `league`, `round` | Normalized competition & kickoff metadata |
| `home_team`, `away_team` | Standardized club names |
| `home_score`, `away_score`, `half_home_score`, `half_away_score` | Official full-time and half-time goals |
| `xg_home`, `xg_away` | Expected goals (xG) |
| `shots_total_*`, `shots_on_target_*`, `corners_*`, `possession_*` | Match technical statistics |
| `total_goals`, `result` | Derived total goals and `H`/`D`/`A` full-time outcome |

## Official Links

- **XG Mind Terminal**: https://xgmind.com/
- **Public Verification Ledger**: https://xgmind.com/performance/
- **Methodology & Calibration**: https://xgmind.com/methodology/
- **Research Blog**: https://xgmind.com/blog/
- **Harvard Dataverse DOI**: https://doi.org/10.7910/DVN/IJ84J8
