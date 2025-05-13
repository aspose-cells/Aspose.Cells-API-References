---
title: DataLabels.ShowCellRange
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Indicates whether showing cell range as the data labels
type: docs
url: /net/aspose.cells.charts/datalabels/showcellrange/
---
## DataLabels.ShowCellRange property

Indicates whether showing cell range as the data labels.

```csharp
public bool ShowCellRange { get; set; }
```

### Examples

```csharp
// Called: series.DataLabels.ShowCellRange = true;
public static void DataLabels_Property_ShowCellRange()
{
    Workbook workbook = new Workbook();
    Worksheet worksheet = workbook.Worksheets[0];
    worksheet.Cells["A1"].PutValue("学历");
    worksheet.Cells["A2"].PutValue("本科");
    worksheet.Cells["A3"].PutValue("专科");
    worksheet.Cells["B1"].PutValue("男生");
    worksheet.Cells["B2"].PutValue(90);
    worksheet.Cells["B3"].PutValue(80);
    worksheet.Cells["C1"].PutValue("女生");
    worksheet.Cells["C2"].PutValue(55);
    worksheet.Cells["C3"].PutValue(63);
    worksheet.Cells["D2"].Formula = $"B2 &\"人\"";
    worksheet.Cells["D3"].Formula = $"B3 &\"人\"";
    worksheet.Cells["E2"].Formula = $"C2 &\"人\"";
    worksheet.Cells["E3"].Formula = $"C3 &\"人\"";

    int chartIndex = worksheet.Charts.Add(ChartType.BarStacked, 0, 5, 20, 15);
    Chart chart = worksheet.Charts[chartIndex];
    chart.Title.IsDeleted = true;
    chart.PlotArea.Area.FillFormat.FillType = FillType.None;
    chart.ChartArea.Area.FillFormat.FillType = FillType.None;
    chart.ValueAxis.MajorGridLines.IsVisible = false;
    chart.ShowLegend = false;
    var chartRange = $"{CellsHelper.CellIndexToName(1, 1)}:{CellsHelper.CellIndexToName(2, 2)}";
    chart.NSeries.Add(chartRange, true);
    for (int i = 1; i <= chart.NSeries.Count; i++)
    {
        var series = chart.NSeries[i - 1];
        series.Name = $"={CellsHelper.CellIndexToName(0, i)}";
        series.Name = $"={CellsHelper.CellIndexToName(0, i)}";
        series.XValues = $"{CellsHelper.CellIndexToName(1, 0)}:{CellsHelper.CellIndexToName(2, 0)}";
        series.DataLabels.LinkedSource = $"{CellsHelper.CellIndexToName(1, i + 2)}:{CellsHelper.CellIndexToName(2, i + 2)}";
        series.DataLabels.NumberFormatLinked = true;
        series.DataLabels.ShowCellRange = true;
        series.DataLabels.Font.Color = Color.White;
    }
    chart.CategoryAxis.IsPlotOrderReversed = true;
    chart.Calculate();
    workbook.Save(Constants.destPath + "example.xlsx");

    workbook = new Workbook(workbook.FileName);
    worksheet = workbook.Worksheets[0];
    chart = worksheet.Charts[0];
    for (int i = 0; i < chart.NSeries.Count; i++)
    {
        var series = chart.NSeries[i];
        Assert.AreEqual(Color.White.ToArgb(), series.DataLabels.Font.Color.ToArgb(), "DataLabel font color");
        foreach (ChartPoint p in series.Points)
        {
            Assert.AreEqual(Color.White.ToArgb(), p.DataLabels.Font.Color.ToArgb(), "DataLabel font color");
        }
    }
}
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


