---
title: TickLabels.RotationAngle
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Represents text rotation angle in clockwise
type: docs
url: /net/aspose.cells.charts/ticklabels/rotationangle/
---
## TickLabels.RotationAngle property

Represents text rotation angle in clockwise.

```csharp
public int RotationAngle { get; set; }
```

### Remarks

0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward.

### Examples

```csharp
// Called: chart.CategoryAxis.TickLabels.RotationAngle = 45;
public void TickLabels_Property_RotationAngle()
{
    Console.WriteLine("TickLabels_Property_RotationAngle()");
    string infn = path + "";
    string outfn = Constants.destPath + "TEST_ChartAxisTickLabelsRotation.xlsx";

    Workbook workbook = new Workbook();
    int sheetIndex = 0;

    Worksheet sheet = workbook.Worksheets[sheetIndex];
    sheet.Cells["A1"].PutValue(150);
    sheet.Cells["A2"].PutValue(100);
    sheet.Cells["A3"].PutValue(150);
    sheet.Cells["B1"].PutValue(33);
    sheet.Cells["B2"].PutValue(20);
    sheet.Cells["B3"].PutValue(50);

    int chartIndex = sheet.Charts.Add(ChartType.Scatter, 15, 0, 35, 10);
    Chart chart = sheet.Charts[chartIndex];
    chart.ValueAxis.MajorGridLines.Style = LineType.Dash;

    chart.NSeries.Add("A1:B3", true);

    ChartFrame plotarea = chart.PlotArea;
    plotarea.Area.BackgroundColor = Color.White;
    plotarea.Area.ForegroundColor = Color.White;

    chart.CategoryAxis.TickLabels.RotationAngle = 45;

    workbook.Save(outfn);

    infn = Constants.destPath + "TEST_ChartAxisTickLabelsRotation.xlsx";
    outfn = Constants.destPath + "TEST_ChartAxisTickLabelsRotation_out.xls";

    workbook = new Workbook(infn);
    workbook.Save(outfn);

}
```

### See Also

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


