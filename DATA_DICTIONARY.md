# Data dictionary

The CSV tables contain serialized, derived experimental metrics. Rows are not independent when they share an object or seed; use the object as the unit for object-level comparisons and retain the nesting fields in the GSO table.

| File | Released scope | Main fields |
| --- | --- | --- |
| `data/fresh_c_matched_control_metrics.csv` | 271 of 300 Fresh C objects across six matched conditions | `object_uid`, `condition`, foreground PSNR/LPIPS/SSIM, edge SSIM, and full-frame PSNR/LPIPS/SSIM |
| `data/fresh_c_equal_budget_contrasts.csv` | Three equal-applied-budget contrasts for the same 271 objects | `object_uid`, `contrast`, and per-object differences for the recorded image metrics |
| `data/fresh_c_c3_fixed_low_contrasts.csv` | C3 minus Fixed Low for the same 271 objects | `object_uid`, foreground PSNR/LPIPS/SSIM, and edge SSIM differences |
| `data/native_mvadapter_metrics.csv` | 43 of 50 native MV-Adapter objects, seven conditions | `object_uid`, `condition`, `seed`, foreground and color/structure metrics |
| `data/geotex_bake10_metrics.csv` | Eight of ten objects in the new GeoTex bake study, eight methods | `object_uid`, `method`, number of unseen views, image metrics, coverage, and UV diagnostics |
| `data/geotex_earlier_bake5_metrics.csv` | Four of five objects in the earlier GeoTex bake study | `evaluation_domain`, `source_id`, `object_uid`, `condition`, `seed`, and image/coverage metrics |
| `data/gso100_view_metrics.csv` | All 100 GSO objects; per-seed and per-view rows | `uid`, `condition`, `seed`, `view`, `role`, and foreground/color metrics |

PSNR and SSIM are higher-is-better metrics; LPIPS and CIEDE2000 are lower-is-better. `fg_` fields refer to foreground-mask measurements. `full_` fields refer to full-frame measurements. Difference tables preserve the contrast direction in the `contrast` field or the source table name; their values are serialized without re-rounding.

`object_uid` and `uid` identify the source object in the study records. The licensed source model files are not included. Full-cohort summaries for Fresh C and all reported inferential results remain in the manuscript and Supplement; the row-level tables here include only records cleared for this limited release.
