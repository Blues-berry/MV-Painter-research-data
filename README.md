# Limited research data for the V5 manuscript

This repository contains a rights-filtered set of object-level results and figure-source metadata for *Timestep-Conditioned Adapter Scaling for Multi-view Diffusion Texture Generation: Control Allocation and Baked Appearance*.

## Scope

The Fresh C source-asset ledger records 300 objects: 271 permit release of derived metrics, 20 permit figure use only, and 9 have unresolved redistribution status. Object-level Fresh C records are included only for the 271 `METRICS_ONLY` objects. Consequently, this deposit does not reproduce every object-level analysis in the manuscript; full-cohort summary statistics remain in the manuscript and Supplement.

The same source-rights filter leaves 43 of 50 native MV-Adapter objects, 8 of 10 GeoTex Bake10 objects, and 4 of 5 earlier GeoTex bake objects in the released tables. The GSO100 table contains all 100 Google Scanned Objects and their per-view results.

The deposit contains derived metrics, data descriptions, and source/license attribution. It does not contain source meshes or textures, generated-image archives, model weights/checkpoints, or participant-level responses. Obtain any source asset directly from its provider and follow the license recorded in `metadata/FIGURE_ASSET_PROVENANCE.csv`.

## Files

- `data/`: filtered object-level tables underlying the reported comparisons.
- `metadata/FIGURE_ASSET_PROVENANCE.csv`: source identity, attribution, license, and source-image hashes for the current main and Supplement figures.
- `metadata/RIGHTS_SCOPE.json`: the asset-rights counts and excluded material categories.
- `metadata/RECORD_COUNTS.json`: source and deposited row/object counts for each table.
- `DATA_DICTIONARY.md`: table columns, conditions, and row-level limits.
- `SHA256SUMS.txt`: integrity hashes for the deposit files.

## License

Original metric tables and documentation in this deposit are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). This license does not extend to third-party source assets; their providers and individual licenses are listed in the provenance metadata.

The GSO source geometry is attributed to Google Research / Google LLC under CC BY 4.0. The Sketchfab model credits and license terms for displayed assets are recorded individually in the provenance metadata and in the manuscript Supplement.

## Citation

The first archived release will receive a DOI. Cite the version-specific DOI shown on the archive record once it is assigned; the versioned GitHub repository is available at <https://github.com/Blues-berry/MV-Painter-research-data>.
