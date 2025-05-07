---
title: Series.Marker
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the marker
type: docs
url: /net/aspose.cells.charts/series/marker/
---
## Series.Marker property

Gets the `marker`.

```csharp
public Marker Marker { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ChartMarkerType.Diamond, chart.NSeries[0].Marker.MarkerStyle, "chart.NSeries[0].MarkerStyle");
private void Property_Marker(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(ChartMarkerType.Diamond, chart.NSeries[0].Marker.MarkerStyle, "chart.NSeries[0].MarkerStyle");
        }
```

### See Also

* class [Marker](../../marker/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


