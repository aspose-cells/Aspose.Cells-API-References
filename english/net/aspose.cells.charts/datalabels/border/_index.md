---
title: DataLabels.Border
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets the border
type: docs
url: /net/aspose.cells.charts/datalabels/border/
---
## DataLabels.Border property

Gets the [`border`](../../../aspose.cells.drawing/line/).

```csharp
public override Line Border { get; }
```

### Examples

```csharp
// Called: chart.NSeries[0].DataLabels.Border.Color = System.Drawing.Color.Red;
public void DataLabels_Property_Border()
{
    Workbook workbook = new Workbook();
    Worksheet sheet = workbook.Worksheets[0];

    sheet.Cells[0, 0].PutValue("A");
    sheet.Cells[0, 1].PutValue("BB");
    sheet.Cells[0, 2].PutValue("CCC");
    sheet.Cells[0, 3].PutValue("DDDD");
    sheet.Cells[0, 4].PutValue("EEEEE");
    sheet.Cells[0, 5].PutValue("FFFFFF");
    sheet.Cells[1, 0].PutValue(100);
    sheet.Cells[1, 1].PutValue(50);
    sheet.Cells[1, 2].PutValue(25);
    sheet.Cells[1, 3].PutValue(12.5);
    sheet.Cells[1, 4].PutValue(6.25);
    sheet.Cells[1, 5].PutValue(3.175);

    int chart_index = sheet.Charts.Add(ChartType.Pie, 5, 5, 5, 5);
    Chart chart = sheet.Charts[chart_index];

    chart.FirstSliceAngle = 10;
    chart.SizeWithWindow = true;
    chart.ShowLegend = false;
    chart.ChartArea.BackgroundMode = BackgroundMode.Transparent;
    chart.ChartArea.Border.IsVisible = false;

    chart.Title.Text = "Great test";
    chart.Title.Font.IsBold = false;
    chart.Title.Font.Size = 24;
    chart.Title.Border.IsVisible = false;
    chart.Title.BackgroundMode = BackgroundMode.Transparent;

    chart.ChartObject.Height = (int)(306 * 1.6);
    chart.ChartObject.Width = (int)(380 * 1.6);

    chart.PlotArea.Height = (int)Math.Round(3270 / 1.5);
    chart.PlotArea.Width = (int)Math.Round(3574 / 1.5);
    chart.PlotArea.X = 280 + (int)((3270 - (int)Math.Round(3270 / 1.5)) / 2);
    chart.PlotArea.Y = 400 + (int)((3574 - (int)Math.Round(3574 / 1.5)) / 2);

    chart.NSeries.Add("A2:F2", false);
    chart.NSeries.CategoryData = "A1:F1";
    chart.NSeries.IsColorVaried = true;

    chart.NSeries[0].DataLabels.Position = LabelPositionType.BestFit;
    chart.NSeries[0].DataLabels.ShowValue = false;
    chart.NSeries[0].DataLabels.ShowCategoryName = true;
    chart.NSeries[0].DataLabels.ShowPercentage = true;
    chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Period;
    chart.ChartArea.Area.ForegroundColor = System.Drawing.Color.Empty;

    //chart.NSeries[0].DataLabels.Border.IsAuto = true;
    chart.NSeries[0].DataLabels.Border.Color = System.Drawing.Color.Red;
    workbook.Save(Constants.destPath + "Test_DataLabelsSeperator.xlsx");
    workbook = new Workbook(Constants.destPath + "Test_DataLabelsSeperator.xlsx");
    Assert.AreEqual(workbook.Worksheets[0].Charts[0].NSeries[0].DataLabels.SeparatorType, DataLabelsSeparatorType.Period);
}
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


