---
layout: page
title: Export to SVG
---

// TODO //

The plots can be exported to SVG by the `SvgExporter` in the OxyPlot core library.

``` csharp
using (var stream = File.Create(fileName))
{
    var exporter = new SvgExporter() { Width = 600, Height = 400 };
    exporter.Export(plotModel, stream);
}
```

- width/height units
- document svg option

Note that SVG can be exported to a standalone document (.svg file) or a HTML5 `<svg\>` element.

### Text measuring

The SVG output requires an `ITextMeasurer` to measure string sizes (rendered width and height). If a text measurer is not specified, the text measurer of the `PdfRenderContext` will be used, which supports simple Type-1 fonts only (Helvetica/Arial, Roman, Courier) limited to WinAnsi encoding. 
To get better text measurements, use one of the render contexts from the platform specific libraries. 