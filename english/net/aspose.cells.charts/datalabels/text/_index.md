---
title: DataLabels.Text
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets or sets the text of data label
type: docs
url: /net/aspose.cells.charts/datalabels/text/
---
## DataLabels.Text property

Gets or sets the text of data label.

```csharp
public override string Text { get; set; }
```

### Examples

```csharp
// Called: pointIndex.DataLabels.Text = &amp;quot;Series 2&amp;quot; + &amp;quot;\n&amp;quot; + &amp;quot;Point &amp;quot; + i;
[Test]
        public void Property_Text()
        {
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Worksheet sheet = workbook.Worksheets[0];
            //Put data
            sheet.Cells[0, 0].PutValue(1);
            sheet.Cells[0, 1].PutValue(2);
            sheet.Cells[0, 2].PutValue(3);

            sheet.Cells[1, 0].PutValue(4);
            sheet.Cells[1, 1].PutValue(5);
            sheet.Cells[1, 2].PutValue(6);

            sheet.Cells[2, 0].PutValue(7);
            sheet.Cells[2, 1].PutValue(8);
            sheet.Cells[2, 2].PutValue(9);

            //Generate the chart
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.ScatterConnectedByLinesWithDataMarker, 5, 1, 24, 10);
            Chart chart = sheet.Charts[chartIndex];

            chart.Title.Text = &quot;Test&quot;;
            chart.CategoryAxis.Title.Text = &quot;X&quot;;
            chart.ValueAxis.Title.Text = &quot;Y&quot;;

            chart.NSeries.CategoryData = &quot;A1:C1&quot;;

            //Insert series
            chart.NSeries.Add(&quot;A2:C2&quot;, false);

            Series series = chart.NSeries[0];

            int pointCount = series.Points.Count;
            for (int i = 0; i &lt; pointCount; i++)
            {
                ChartPoint pointIndex = series.Points[i];

                pointIndex.DataLabels.Text = &quot;Series 1&quot; + &quot;\n&quot; + &quot;Point &quot; + i;
            }

            //Insert series
            chart.NSeries.Add(&quot;A3:C3&quot;, false);

            series = chart.NSeries[1];

            pointCount = series.Points.Count;
            for (int i = 0; i &lt; pointCount; i++)
            {
                ChartPoint pointIndex = series.Points[i];

                pointIndex.DataLabels.Text = &quot;Series 2&quot; + &quot;\n&quot; + &quot;Point &quot; + i;
            }

            workbook.Save(Constants.destPath + &quot;Cellsnet43116.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Cellsnet43116.xlsx&quot;);
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.Text, &quot;Series 1&quot; + &quot;\n&quot; + &quot;Point &quot; + 0);

        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


