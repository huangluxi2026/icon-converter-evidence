# One-PNG site-icon result-page benchmark

## Scope

This dataset is a single dated run of ten English-language Google result pages for the query `site icon generator`. The source is the published test record at https://pngtoicotool.com/site-icon-generator-benchmark.

## Protocol

- Test date: 2026-10-18.
- Input: one original 512 × 512 PNG with transparent corners; the upper-left pixel alpha was 0 and the center pixel alpha was 255.
- Browser and OS: Windows 11 Pro; Chrome 155.0.8059.84.
- Search query parameters: `hl=en`, `gl=us`, `pws=0`; physical search location was not verified.
- One default route per result page; no sign-in. Where a download completed, the downloaded artifact was inspected locally.
- If the upload/download flow did not complete, output-dependent fields are `Not measured`; the recorded cell says where the run stopped.

## Limits

This is one input and one browser session, not a universal feature or quality verdict. Some entries are design platforms rather than converters. The visible upload-size limit was recorded only when shown during this run; it was not exhaustively checked across each service. Mobile behavior, visual tab rendering, and generation time were not measured. The companion video is a result walkthrough and does not rerun the ten tools live.

## Data fields

`site-icon-generator-one-png.csv` preserves the rank order and comparison fields from the source table. `Not measured` is not an inferred negative result.

