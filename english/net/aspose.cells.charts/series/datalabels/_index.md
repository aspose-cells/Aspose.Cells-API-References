---
title: Series.DataLabels
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the DataLabels object for the specified ASeries
type: docs
url: /net/aspose.cells.charts/series/datalabels/
---
## Series.DataLabels property

Represents the DataLabels object for the specified ASeries.

```csharp
public DataLabels DataLabels { get; }
```

### Examples

```csharp
// Called: series.DataLabels.LinkedSource = null; // LinkedSource was null already before this.
public void Series_Property_DataLabels()
{
    var workbook = new Workbook();
    Worksheet chartSheet = workbook.Worksheets[workbook.Worksheets.Add(SheetType.Chart)];
    Worksheet ws = workbook.Worksheets[0];
    ws.Cells["A1"].PutValue("Products");
    ws.Cells["B1"].PutValue("Users");
    ws.Cells["A2"].PutValue("Aspose.Cells");
    ws.Cells["B2"].PutValue(10000);
    ws.Cells["A3"].PutValue("Aspose.Slides");
    ws.Cells["B3"].PutValue(8000);
    ws.Cells["A4"].PutValue("Aspose.Words");
    ws.Cells["B4"].PutValue(12000);

    Chart chart = chartSheet.Charts[chartSheet.Charts.Add(ChartType.Pie, 7, 0, 20, 6)];

    Series series = chart.NSeries[chart.NSeries.Add("=Sheet1!$B$2:$B$4", true)];
    series.XValues = "=Sheet1!$A$2:$A$4";

    series.DataLabels.LinkedSource = null; // LinkedSource was null already before this. 
    Util.ReSave(workbook, SaveFormat.Xlsx); //here should not give exception when openning the resaved xlsx
}
```

### See Also

* class [DataLabels](../../datalabels/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


