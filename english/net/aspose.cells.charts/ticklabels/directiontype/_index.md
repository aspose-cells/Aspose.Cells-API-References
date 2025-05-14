---
title: TickLabels.DirectionType
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Gets and sets the direction of text
type: docs
url: /net/aspose.cells.charts/ticklabels/directiontype/
---
## TickLabels.DirectionType property

Gets and sets the direction of text.

```csharp
public ChartTextDirectionType DirectionType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.CategoryAxis.TickLabels.DirectionType, ChartTextDirectionType.Vertical, "TickLabels.DirectionType");
public void TickLabels_Property_DirectionType()
{
    // Instantiating a Workbook object
    Workbook workbook = new Workbook();
    WorksheetCollection worksheets = workbook.Worksheets;

    Worksheet worksheet = worksheets[0];

    Cells cells = worksheet.Cells;

    cells["A1"].Value = (50);
    cells["A2"].Value = (100);
    cells["A3"].Value = (150);
    cells["A4"].Value = (200);
    cells["B1"].Value = (60);
    cells["B2"].Value = (32);
    cells["B3"].Value = (50);
    cells["B4"].Value = (40);
    cells["C1"].Value = ("清华");
    cells["C2"].Value = ("北大");

    cells["C3"].Value = ("人大");
    cells["C4"].Value = ("科大");

    ChartCollection charts = worksheet.Charts;
    int chartIndex = charts.Add(ChartType.Column, 5, 0, 15, 5);
    Chart chart = charts[chartIndex];
    // Integer t=ChartTextDirectionType.VERTICAL;

    // Adding NSeries (chart data source) to the chart ranging from "A1"
    // cell to "B4"
    SeriesCollection nSeries = chart.NSeries;
    nSeries.Add("A1:B4", true);

    // Setting the data source for the category data of NSeries
    nSeries.CategoryData = ("C1:C4");

    chart.CategoryAxis.TickLabels.DirectionType = (ChartTextDirectionType.Vertical);

    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(workbook.FileName);
    chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.CategoryAxis.TickLabels.DirectionType, ChartTextDirectionType.Vertical, "TickLabels.DirectionType");
}
```

### See Also

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


