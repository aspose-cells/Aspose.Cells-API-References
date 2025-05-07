---
title: Marker.Border
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Gets the border
type: docs
url: /net/aspose.cells.charts/marker/border/
---
## Marker.Border property

Gets the [`border`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; }
```

### Examples

```csharp
// Called: chart.NSeries[0].Points[intPointIndex].Marker.Border.Color = Color.Yellow;
[Test]
        public void Property_Border()
        {
            Console.WriteLine("Property_Border()");
            string outfn = Constants.destPath + "TEST_TextBox2_out.xlsx";

            Workbook workbook = new Workbook();

            int sheetIndex = 0;

            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            worksheet.Cells["A1"].PutValue(150);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(33);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            int intPointIndex = 0;

            chart.NSeries[0].Points[intPointIndex].Marker.Border.Color = Color.Yellow;
            chart.NSeries[0].Points[intPointIndex].Marker.Area.ForegroundColor = Color.Green;
            chart.NSeries[0].Points[intPointIndex].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Points[intPointIndex].Marker.MarkerSize = 16;
            chart.NSeries[0].Points[intPointIndex].DataLabels.ShowValue = true;
            //chart.NSeries[0].Points[intPointIndex].DataLabels.Text = "mmm";
            chart.NSeries[0].Points[intPointIndex].DataLabels.Font.Color = Color.Blue;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Font.Name = "Arial";
            chart.NSeries[0].Points[intPointIndex].DataLabels.Font.Size = 16;
            //chart.NSeries[0].Points[intPointIndex].DataLabels.AutoScaleFont = false;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Position = LabelPositionType.Below;

            TextBox tb = chart.Shapes.AddTextBoxInChart(500, 500, 500, 500);
            tb.Text = "i am text box";

            workbook.Save(outfn);
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


