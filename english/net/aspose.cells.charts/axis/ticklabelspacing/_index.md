---
title: Axis.TickLabelSpacing
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the number of categories or series between tickmark labels. Applies only to category and series axes
type: docs
url: /net/aspose.cells.charts/axis/ticklabelspacing/
---
## Axis.TickLabelSpacing property

Represents the number of categories or series between tick-mark labels. Applies only to category and series axes.

```csharp
public int TickLabelSpacing { get; set; }
```

### Remarks

The number must be between 1 and 31999.

### Examples

```csharp
// Called: chart.CategoryAxis.TickLabelSpacing = 60;
public void Axis_Property_TickLabelSpacing()
{
    Workbook workbook = new Workbook();

    int index = workbook.Worksheets.Add();
    Worksheet worksheet = workbook.Worksheets[index];

    worksheet.Cells[0, 0].PutValue("Defect Case");
    worksheet.Cells[0, 1].PutValue("Qty");

    worksheet.Cells[1, 0].PutValue("Cut not straight");
    worksheet.Cells[1, 1].PutValue(9);

    worksheet.Cells[2, 0].PutValue("No defect found");
    worksheet.Cells[2, 1].PutValue(7);

    worksheet.Cells[3, 0].PutValue("Product not made by FLC");
    worksheet.Cells[3, 1].PutValue(3);

    worksheet.Cells[4, 0].PutValue("Sample lost");
    worksheet.Cells[4, 1].PutValue(3);

    worksheet.Cells[5, 0].PutValue("Incorrect hose cut length");
    worksheet.Cells[5, 1].PutValue(3);

    worksheet.Cells[6, 0].PutValue("Mechanical failure");
    worksheet.Cells[6, 1].PutValue(2);

    worksheet.Cells[7, 0].PutValue("Missing quantity");
    worksheet.Cells[7, 1].PutValue(1);

    worksheet.Cells[8, 0].PutValue("Accessories");
    worksheet.Cells[8, 1].PutValue(1);

    int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.ParetoLine, 5, 0, 40, 19);
    string dataArea = "B2: B9";
    string categoryArea = "A2: A9";

    Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
    chart.NSeries.Add(dataArea, true);
    chart.PlotArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Transparent;
    chart.PlotArea.Area.ForegroundColor = Color.Transparent;
    chart.ChartArea.Area.ForegroundColor = Color.FromArgb(242, 242, 242);
    chart.ChartArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Automatic;
    chart.ChartArea.Font.Color = Color.DarkBlue;

    chart.CategoryAxis.CategoryType = Aspose.Cells.Charts.CategoryType.CategoryScale;
    chart.CategoryAxis.TickLabelSpacing = 60;

    chart.NSeries.CategoryData = categoryArea;
    chart.NSeries[0].Name = "= B1";

    chart.ShowLegend = false;

    workbook.Save(Constants.destPath + "example.xlsx", SaveFormat.Xlsx);
}
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


