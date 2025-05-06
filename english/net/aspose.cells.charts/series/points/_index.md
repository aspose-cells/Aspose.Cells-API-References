---
title: Series.Points
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the collection of points in a series in a chart
type: docs
url: /net/aspose.cells.charts/series/points/
---
## Series.Points property

Gets the collection of points in a series in a chart.

```csharp
public ChartPointCollection Points { get; }
```

### Remarks

When the chart is Pie of Pie or Bar of Pie, the last point is other point in first pie plot.

### Examples

```csharp
// Called: chart.NSeries[0].Points[intPointIndex].DataLabels.Position = LabelPositionType.Below;
[Test]
        public void Property_Points()
        {
            Console.WriteLine(&quot;Property_Points()&quot;);
            string infn = path + &quot;TEST_ChartPointDataLabel.xlsx&quot;;
            string outfn = Constants.destPath + &quot;TEST_ChartPointDataLabel_out.xlsx&quot;;


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

            //chart.NSeries[0].Points[intPointIndex].DataLabels.ShowValue = true;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Text = &quot;mmm&quot;;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Font.Color = Color.Blue;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Font.Name = &quot;Arial&quot;;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Font.Size = 16;
            //chart.NSeries[0].Points[intPointIndex].DataLabels.AutoScaleFont = false;
            chart.NSeries[0].Points[intPointIndex].DataLabels.Position = LabelPositionType.Below;

            workbook.Save(outfn);
        }
```

### See Also

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


