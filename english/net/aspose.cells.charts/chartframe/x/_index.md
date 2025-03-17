---
title: ChartFrame.X
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartframe/x/
---
## ChartFrame.X property

Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartFrame.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int X { get; set; }
```

### Remarks

How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000d;

NOTE: This member is now obsolete. Please use ChartFrame.XRatioToChart property, instead. X = XRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


