---
layout: page
title: Features
---

// TODO //

### Platforms

Interactive controls are implemented on the following platforms

- WPF
- Windows Forms
- Silverlight
- Windows Store App
- GTK#
- Xamarin.Android
- Xamarin.iOS
- Xamarin.Mac

### Plot types

- XY (horizontal and vertical axes)
- Cartesian (same scale on X and Y axis)
- Polar
- Pie chart

### Axes

| Linear | |
| Logarithmic | |
| CategoryAxis | for bar and column series |
| Date/time (alpha) | |
| Time span (alpha) | |
| LinearColorAxis | for heat maps and scatter series|
| AngleAxis | for polar plots|
| MagnitudeAxis | for polar plots|

### Series

The following types of series are included in the core library

// TODO - add missing types //

|| Use || to create |
| LineSeries | line plots (graphs) |
| ScatterSeries | scatter plots (scatterplots, scattergraphs)|
| AreaSeries | area plots|
| StemSeries | stem charts|
| StairStepSeries | stairstep charts|
| HighLowSeries | open-high-low-close (OHLC) charts|
| CandlestickSeries | candlestick charts|
| BarSeries | bar charts|
| ColumnSeries | column charts|
| PieSeries | pie charts|
| HeatMapSeries | heat maps|
| ContourSeries | contour plots|

Different types of series can be added to the same plot.

It is easy to extend with custom series types.

### Annotations

// TODO - add missing types //

|| Annotation || Description |
| LineAnnotation | |
| ArrowAnnotation| |

### Output file formats

The plots can be exported to the following raster and vector file formats:

- [PNG](./export-png)
- [SVG](./export-svg)
- [PDF](./export-pdf)
- XPS

### Limitations

- the plot controls are not subscribing to `INotifyPropertyChanged` and `INotifyCollectionChanged` events. You must manually refresh the plots when changing your data.
- no animations
- no gradient or hatch brushes
