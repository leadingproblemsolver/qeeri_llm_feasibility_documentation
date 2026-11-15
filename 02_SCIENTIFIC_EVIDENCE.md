# Scientific evidence and epistemic boundaries

## Defensible statements
1. Evaporative-pad outlet temperature may be estimated with `T_pad = T_db - ε(T_db - T_wb)`. For *illustrative inputs* 38 °C / 24 °C and ε=0.85, **T_pad=26.1 °C**. This does **not** predict crop-zone temperature, equipment capacity, yield, or site feasibility. Source of general method: UF/IFAS AE069.
2. The Al Khor research of Ghani et al. includes simulated ventilation/thermal effects and reference conditions. **Do not transfer numerical Al Khor findings as Al-Shahaniya measurements.** DOI: 10.1080/23744731.2019.1634421.
3. Shannak, Kafi et al., *Qatari Crop Performance Index* (2026), Tables 14–15, report Qatar agricultural tomato system comparisons. Values per **dunum**, not site-specific forecasts:

| System | Yield (t/dunum) | Electricity (kWh/dunum) | Water (m³/dunum) |
|---|---:|---:|---:|
| Open field | 5.3 | 1,702 | 1,000 |
| Soil greenhouse, uncooled | 9.6 | 3,845 | 1,500 |
| Soil greenhouse, cooled | 10.4 | 15,000 | 2,000 |
| Soilless greenhouse, uncooled | 14.0 | 3,845 | 1,500 |
| Soilless greenhouse, cooled | 16.0 | 27,160 | 1,500 |

  Source: Shannak et al. 2026, DOI 10.1016/j.nexus.2026.100787. Exact scenario definitions and observation/model status should be checked against the publication before independent quantitative reuse.
4. Mahmood et al. 2022 examines a **semi-closed** Al-Shahaniya greenhouse; bibliographic reference exists but precise numerical inputs/claims from its full text remain unverified. DOI 10.1080/01430750.2022.2088617.
5. KAHRAMAA electricity code **2016** was identified, but current applicability and any derived design compliance require professional review. FAO principles are methodological, not Qatar-specific installation permission.

## Data inventory
| Input | Available | Evidence class |
|---|---|---|
| Original scientific articles | Identified, selected passages examined | Published; source-specific |
| Sizing workbook: 400 m² and 46/28 °C assumptions | Input cells; derived result cells blank in inspected file | **ASSUMED / NOT EXECUTED** |
| Soil samples (60 records) | Synthetic file | **SYNTHETIC** |
| Matched UAV/lab soil data | Not found | **MISSING** |
| Instrumented greenhouse climate and water data | Not established | **MISSING** |
| ERA5-Land selected point time series | Methodology only | **NOT COLLECTED** |
| Actual plant-height temperature or crop yield | Not established | **MISSING** |
| Electricity, water tariff, quotations, CAPEX and OPEX for target site | Not established | **MISSING** |

## Acceptable claim vocabulary
`SOURCE_REPORTED`, `CALCULATED_ILLUSTRATIVE`, `SOURCE_PENDING_REVIEW`, `SYNTHETIC`, `NOT_FOUND`, `HUMAN_REVIEW_PENDING`.

**Conclusion:** Literature supports a provisional constraint inventory and calculations, not construction advice or investment approval.