---
title: Chart.NSeries
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets a SeriesCollection collection representing the data series in the chart
type: docs
url: /net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

Gets a [`SeriesCollection`](../../seriescollection/) collection representing the data series in the chart.

```csharp
public SeriesCollection NSeries { get; }
```

### Examples

```csharp
// Called: chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);
public static Workbook Chart_Property_NSeries(Workbook workbook)
        {
            workbook = new Workbook(Constants.sourcePath + "Charts\\Line\\Line.xls");
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[sheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 2, 25, 11)];
            chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);
            return workbook;
        }
```

### See Also

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


