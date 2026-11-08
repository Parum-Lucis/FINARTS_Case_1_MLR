# data/

Inputs for `report/Case_Study_Report.Rmd`. The report reads everything in `raw/` through
`here::here("data", "raw", ...)`, so it works from any working directory. Nothing in `raw/` is edited by hand.

## raw/

| File | Contents | Used by the report |
|:--|:--|:--|
| PH_10Y_GS_YIELD_1725.xlsx | Philippine 10-year government bond yield, daily, Dec 2017 to Dec 2025 (LSEG Workplace) | yes |
| PSEI_1725.xlsx | PSEi daily close, Dec 2017 to Dec 2025 (LSEG Workplace) | yes |
| USDPHP_1725.xlsx | USD/PHP daily mid price, Dec 2017 to Dec 2025 (LSEG Workplace) | yes |
| PH_RRP_1725.xlsx | BSP reverse repurchase (RRP) rate by effective date | yes |
| PH RRP TEXT.xlsx | Presumably the RRP announcement text the RRP series was parsed from (the Rmd notes the parsing was done with Claude Sonnet 5.5) | no, provenance only |
| PH_CPI_YY_1626.xlsx | Philippine CPI, year-on-year %, monthly (file name says 2016-2026) | yes |
| PH_M3_YY_1626.xlsx | Philippine M3 money supply, year-on-year %, monthly | yes |
| PH_Manufacturing_Production_YY_1626.xlsx | Philippine manufacturing production, year-on-year %, monthly | yes |
| fred_daily_snapshot.csv | WTI crude (DCOILWTICO), S&P 500 (SP500) and VIX (VIXCLS), daily, from FRED | yes |
| fred_daily_snapshot_info.txt | When and how the FRED snapshot was downloaded | no |

## raw/_unused/

`PSEI_1825.xlsx`, `USDPHP_1825.xlsx` and `PH_10Y_GS_YIELD_1825.xlsx`: alternative extracts (file names say 2018-2025).
The report reads the `_1725` files instead, so these are parked here, not deleted.

## To fill in

Retrieval dates for the LSEG files are not recorded anywhere. Add them to the table above.