---
title: Chart.ValueAxis
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts Y axis
type: docs
url: /net/aspose.cells.charts/chart/valueaxis/
---
## Chart.ValueAxis property

Gets the chart's Y axis.

```csharp
public Axis ValueAxis { get; }
```

### Examples

```csharp
// Called: chart.ValueAxis.MajorGridLines.Style = LineType.Dash;
[Test]
        public void Property_ValueAxis()
        {
            Console.WriteLine(&quot;Property_ValueAxis()&quot;);
            string infn = path + &quot;&quot;;
            string outfn = Constants.destPath + &quot;TEST_ChartAxisTickLabelsRotation.xlsx&quot;;

            Workbook workbook = new Workbook();
            int sheetIndex = 0;

            Worksheet sheet = workbook.Worksheets[sheetIndex];
            sheet.Cells[&quot;A1&quot;].PutValue(150);
            sheet.Cells[&quot;A2&quot;].PutValue(100);
            sheet.Cells[&quot;A3&quot;].PutValue(150);
            sheet.Cells[&quot;B1&quot;].PutValue(33);
            sheet.Cells[&quot;B2&quot;].PutValue(20);
            sheet.Cells[&quot;B3&quot;].PutValue(50);

            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 15, 0, 35, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.ValueAxis.MajorGridLines.Style = LineType.Dash;

            chart.NSeries.Add(&quot;A1:B3&quot;, true);

            ChartFrame plotarea = chart.PlotArea;
            plotarea.Area.BackgroundColor = Color.White;
            plotarea.Area.ForegroundColor = Color.White;

            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            workbook.Save(outfn);

            infn = Constants.destPath + &quot;TEST_ChartAxisTickLabelsRotation.xlsx&quot;;
            outfn = Constants.destPath + &quot;TEST_ChartAxisTickLabelsRotation_out.xls&quot;;

            workbook = new Workbook(infn);
            workbook.Save(outfn);

        }
```

### See Also

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


