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
// Called: chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Diamond;
[Test]
        public void Property_Marker()
        {
            Workbook workbook = new Workbook();
            workbook = TestLine.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Diamond;

            checkChartMarkerType_Diamond(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkChartMarkerType_Diamond(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkChartMarkerType_Diamond(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [Marker](../../marker/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


