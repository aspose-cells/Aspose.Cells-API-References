---
title: DataLabels.NumberFormat
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Represents the format string for the DataLabels object
type: docs
url: /net/aspose.cells.charts/datalabels/numberformat/
---
## DataLabels.NumberFormat property

Represents the format string for the DataLabels object.

```csharp
public string NumberFormat { get; set; }
```

### Examples

```csharp
// Called: datalabels.NumberFormat = "0%";
[Test]
        public void Property_NumberFormat()
        {
            Console.WriteLine("Property_NumberFormat()");
            string outfn = Constants.destPath + "TEST_MovePlotArea_out.xlsx";

            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook();
            Aspose.Cells.Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "Data";
            Aspose.Cells.Cells cells = workbook.Worksheets[0].Cells;
            workbook.ChangePalette(Color.Orange, 53);
            workbook.ChangePalette(Color.LightBlue, 54);
            workbook.ChangePalette(Color.LightCoral, 55);
            workbook.ChangePalette(Color.Indigo, 52);
            Color[] colors = workbook.Colors;
            cells["A1"].PutValue("Excelsior lasalle property fund LLC ");
            cells["A2"].PutValue("Excelsior lasalle property fund\n LLC property fund LLC ");
            cells["A3"].PutValue("Germany"); cells["A4"].PutValue("England");
            cells["A5"].PutValue("Sweden"); cells["B1"].PutValue("Sale");
            cells["B2"].PutValue(0.32); cells["B3"].PutValue(0.62); cells["B4"].PutValue(0.06);
            cells["B5"].PutValue(0.06); int chartIndex = 0;
            chartIndex = sheet.Charts.Add(ChartType.Pie, 1, 3, 25, 12);
            Chart c = sheet.Charts[chartIndex]; c.Legend.Border.IsVisible = false;
            c.Legend.AutoScaleFont = true; c.Legend.AutoScaleFont = false;
            c.Legend.TextFont.Name = "Arial"; c.Legend.TextFont.Size = 7;
            c.Legend.Position = LegendPositionType.Right;
            c.ChartArea.BackgroundMode = BackgroundMode.Transparent;
            c.NSeries.Add("Data!B2:B5", true); c.NSeries.CategoryData = "Data!A2:A5";
            DataLabels datalabels;
            for (int i = 0; i < c.NSeries.Count; i++)
            {
                datalabels = c.NSeries[i].DataLabels;
                datalabels.ShowPercentage = true;
                datalabels.NumberFormat = "0%";
                datalabels.Position = LabelPositionType.OutsideEnd;
                datalabels.TextFont.Name = "Arial"; datalabels.TextFont.Size = 7;
            }
            c.PlotArea.X = 0; c.PlotArea.Y = 700; workbook.Save(outfn);
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


