---
title: Marker.MarkerStyle
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Represents the marker style. Applies to line chart scatter chart or radar chart
type: docs
url: /net/aspose.cells.charts/marker/markerstyle/
---
## Marker.MarkerStyle property

Represents the marker style. Applies to line chart, scatter chart, or radar chart.

```csharp
public ChartMarkerType MarkerStyle { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ChartMarkerType.Dash, chart.NSeries[0].Marker.MarkerStyle, &amp;quot;chart.NSeries[0].MarkerStyle&amp;quot;);
private void Property_MarkerStyle(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet2&quot;];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(ChartMarkerType.Dash, chart.NSeries[0].Marker.MarkerStyle, &quot;chart.NSeries[0].MarkerStyle&quot;);
        }
```

### See Also

* enum [ChartMarkerType](../../chartmarkertype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


