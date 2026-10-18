# Icon Converter Evidence

A small set of measured ICO and favicon outputs, plus an ICNS layer map parsed from a file created by the browser converter.

## Files

- `png-to-ico-output-matrix.csv` — one row per saved ICO in the published PNG-to-ICO converter comparison. It records the source PNG dimensions, output byte length, frame count, frame dimensions, and payload encoding.
- `favicon-extractor-32px-comparison.csv` — the selected 32-pixel results from two favicon extractors and the separately observed homepage Apple Touch and manifest declarations. Failed returned links are marked as not completed.
- `icns-layer-size-sample.csv` — chunk codes, embedded PNG dimensions, and chunk byte lengths read from one ICNS file generated with the site’s PNG-to-ICNS tool.
- `site-icon-generator-one-png.csv` — a ten-result-page comparison from one unchanged transparent PNG. Output-dependent fields remain marked not measured when no artifact was recovered.
- `site-icon-generator-benchmark-method.md` — the dated protocol, environment, and limits for that one-PNG run.

Open the CSV files in a spreadsheet or read them with any CSV parser. Dimensions are in pixels; byte fields are file or chunk lengths as named in their headers.

## Provenance and limits

The ICO matrix summarizes files downloaded and decoded in the PNG-to-ICO downloaded-file lab. Its four input images and per-frame measurements are described on the site page `png-to-ico-shape-matrix`. Each row describes an observed output and its recorded settings; it is not a universal guarantee for a converter.

The favicon comparison is the table on `favicon-extractor`, covering two extractors’ selected 32-pixel result links and separate homepage declarations. A returned-link 404 means that result was not completed; it does not mean the target site has no favicon. Homepage declarations are not credited to either extractor.

The ICNS map is a single locally generated sample parsed from its ICNS container and PNG IHDR chunks. It describes that sample only; other ICNS files can contain different entries or older image encodings.

The one-PNG result-page comparison uses one 512 × 512 transparent image, one default route per result page, and one Windows Chrome session. The [published test record](https://pngtoicotool.com/site-icon-generator-benchmark) includes observed stop points; a failed file chooser or blocked download is not treated as a measured output.

These measured files and browser tools are maintained at [pngtoicotool.com](https://pngtoicotool.com/).
