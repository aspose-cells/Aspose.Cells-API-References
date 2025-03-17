---
title: ChartFrame.Width
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets or sets the width of frame in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartframe/width/
---
## ChartFrame.Width property

Gets or sets the width of frame in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartFrame.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Width { get; set; }
```

### Remarks

How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000d;

NOTE: This member is now obsolete. Please use ChartFrame.WidthRatioToChart property, instead. Width = WidthRatioToChart * 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


