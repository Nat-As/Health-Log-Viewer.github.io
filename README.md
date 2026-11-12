# Health-Log-Viewer
Visualize system health log csv files

Website available at: [https://nat-as.github.io/Health-Log-Viewer.github.io/](https://nat-as.github.io/Health-Log-Viewer.github.io/)

# Features
+ Graph Health Log CSVs with auto scaling
+ Select multiple series to plot simultaneously
+ Added zoom feature - shift + click to select zoom area
+ Automatic field type detection (timestamp, boolean, state/enum, integer, numeric) with units inferred from column suffixes (`_C`, `_V`, `_A`, `_W`, `_m`, `_s`, `_%`, ...)
+ Y axes labeled by unit (e.g. `Temperature (°C)`), up to two axes; booleans/states plot as step lines with the lowest state 10% above the bottom and the highest 10% below the top
+ Idle gaps (system off / no data) are collapsed on the time axis so each startup gets its own space; dashed lines and labels mark each discontinuity and its duration. Threshold is automatic or selectable
+ Handles large logs: min/max decimation and no per-point markers on dense series
