# CSV Waveform Viewer

A minimal, browser-only viewer for time-series CSV files.

## Use

1. Open `index.html` in a modern browser.
2. Select a CSV file.
3. Choose the time and signal columns, then enter the signal unit if needed.

The included `example.csv` is synthetic data. Your selected CSV stays on your computer: this page does not upload data or contact a server.

## CSV format

The first row must be headers. Use one numeric time column and one or more numeric signal columns.

```csv
time_s,channel_1_mV,channel_2_mV
0.0,0.00,0.30
0.5,0.45,0.68
```

## Scope

This repository is intentionally a viewer only. It does not include experimental data, MED64 conversion, frequency-domain analysis, peak detection, or slow-wave interpretation.

## License

MIT
