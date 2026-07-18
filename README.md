# Multichannel Slow-Wave Dashboard

A browser-only, integrated dashboard for 64-channel time-series CSV files.

## Use

1. Open `index.html` in a modern browser.
2. Select a CSV with one time column followed by 64 channel columns.
3. Inspect the waveform, 2D map, 3D potential surface, and per-channel metrics.
4. To compare recordings, select up to six files in the 3D comparison CSV control. Each surface has its own time slider and uses a shared color and height scale.

The initial dashboard display uses synthetic data. Your selected CSV stays on your computer: this page does not upload data or contact a server.

## CSV format

The first row must be headers. The first column must be numeric time values, followed by up to 64 numeric channel columns. Voltage data smaller than 0.1 in absolute value are displayed as mV; otherwise the original numeric unit is preserved.

```csv
time_s,ch1,ch2,...,ch64
0.0,0.00,0.30,...,-0.12
0.5,0.45,0.68,...,0.08
```

## Scope

The dashboard includes local, exploratory visualization and summary calculations: waveform playback, 2D and 3D 8x8 potential maps, peak-to-peak amplitude, peak-derived frequency, FFT-based dominant frequency, and related signal summaries. It does not include experimental data, MED64 conversion, laboratory metadata, or claims of biological interpretation.

## License

MIT
