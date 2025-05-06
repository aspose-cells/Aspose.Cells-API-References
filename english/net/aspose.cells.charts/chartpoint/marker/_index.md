---
title: ChartPoint.Marker
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Gets the  marker
type: docs
url: /net/aspose.cells.charts/chartpoint/marker/
---
## ChartPoint.Marker property

Gets the ` marker`.

```csharp
public Marker Marker { get; }
```

### Examples

```csharp
// Called: chart.NSeries[0].Points[intPointIndex].Marker.MarkerStyle = ChartMarkerType.Circle;
[Test]
        public void Property_Marker()
        {
            Console.WriteLine(&quot;Property_Marker()&quot;);
            string outfn = Constants.destPath + &quot;TEST_TextBox2_out.xlsx&quot;;

            Workbook workbook = new Workbook();

            int sheetIndex = 0;

            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            worksheet.Cells[&quot;A1&quot;].PutValue(150);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(33);
            worksheet.Cells[&quot;B2&quot;].PutValue(20);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add(&quot;A1:B3&quot;, true);
            int intPointIndex = 0;

            chart.NSeries[0].Points[intPointIndex].Marker.Border.Color = Color.Yellow;
            chart.NSeries[0].Points[intPointIndex].Marker.Area.ForegroundColor = Color.Green;
            chart.NSeries[0].Points[intPointIndex].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Points[intPointIndex].Marker.MarkerSize = 16;
            chart.NSeries[0].Points[intPointIndex].DataLabels.ShowValue = true;
            //chart.NSeries[0].Points[intPointIndex].DataLabels.Text = &quot;mmm&quot;;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Font.Color = Color.Blue;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Font.Name = &quot;Arial&quot;;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Font.Size = 16;
            //chart.NSeries[0].Points[intPointIndex].DataLabels.AutoScaleFont = false;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Position = LabelPositionType.Below;

            TextBox tb = chart.Shapes.AddTextBoxInChart(500, 500, 500, 500);
            tb.Text = &quot;i am text box&quot;;

            workbook.Save(outfn);
        }
```

### See Also

* class [Marker](../../marker/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


