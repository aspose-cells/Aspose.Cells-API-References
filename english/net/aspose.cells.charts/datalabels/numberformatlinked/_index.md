---
title: DataLabels.NumberFormatLinked
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. True if the number format is linked to the cells so that the number format changes in the labels when it changes in the cells
type: docs
url: /net/aspose.cells.charts/datalabels/numberformatlinked/
---
## DataLabels.NumberFormatLinked property

True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

```csharp
public bool NumberFormatLinked { get; set; }
```

### Examples

```csharp
// Called: series.DataLabels.NumberFormatLinked = true;
[Test]
        public static void Property_NumberFormatLinked()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;学历&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;本科&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;专科&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;男生&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(90);
            worksheet.Cells[&quot;B3&quot;].PutValue(80);
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;女生&quot;);
            worksheet.Cells[&quot;C2&quot;].PutValue(55);
            worksheet.Cells[&quot;C3&quot;].PutValue(63);
            worksheet.Cells[&quot;D2&quot;].Formula = $&quot;B2 &amp;\&quot;人\&quot;&quot;;
            worksheet.Cells[&quot;D3&quot;].Formula = $&quot;B3 &amp;\&quot;人\&quot;&quot;;
            worksheet.Cells[&quot;E2&quot;].Formula = $&quot;C2 &amp;\&quot;人\&quot;&quot;;
            worksheet.Cells[&quot;E3&quot;].Formula = $&quot;C3 &amp;\&quot;人\&quot;&quot;;

            int chartIndex = worksheet.Charts.Add(ChartType.BarStacked, 0, 5, 20, 15);
            Chart chart = worksheet.Charts[chartIndex];
            chart.Title.IsDeleted = true;
            chart.PlotArea.Area.FillFormat.FillType = FillType.None;
            chart.ChartArea.Area.FillFormat.FillType = FillType.None;
            chart.ValueAxis.MajorGridLines.IsVisible = false;
            chart.ShowLegend = false;
            var chartRange = $&quot;{CellsHelper.CellIndexToName(1, 1)}:{CellsHelper.CellIndexToName(2, 2)}&quot;;
            chart.NSeries.Add(chartRange, true);
            for (int i = 1; i &lt;= chart.NSeries.Count; i++)
            {
                var series = chart.NSeries[i - 1];
                series.Name = $&quot;={CellsHelper.CellIndexToName(0, i)}&quot;;
                series.Name = $&quot;={CellsHelper.CellIndexToName(0, i)}&quot;;
                series.XValues = $&quot;{CellsHelper.CellIndexToName(1, 0)}:{CellsHelper.CellIndexToName(2, 0)}&quot;;
                series.DataLabels.LinkedSource = $&quot;{CellsHelper.CellIndexToName(1, i + 2)}:{CellsHelper.CellIndexToName(2, i + 2)}&quot;;
                series.DataLabels.NumberFormatLinked = true;
                series.DataLabels.ShowCellRange = true;
                series.DataLabels.Font.Color = Color.White;
            }
            chart.CategoryAxis.IsPlotOrderReversed = true;
            chart.Calculate();
            workbook.Save(Constants.destPath + &quot;CELLSNET-48696.xlsx&quot;);

            workbook = new Workbook(workbook.FileName);
            worksheet = workbook.Worksheets[0];
            chart = worksheet.Charts[0];
            for (int i = 0; i &lt; chart.NSeries.Count; i++)
            {
                var series = chart.NSeries[i];
                Assert.AreEqual(Color.White.ToArgb(), series.DataLabels.Font.Color.ToArgb(), &quot;DataLabel font color&quot;);
                foreach (ChartPoint p in series.Points)
                {
                    Assert.AreEqual(Color.White.ToArgb(), p.DataLabels.Font.Color.ToArgb(), &quot;DataLabel font color&quot;);
                }
            }
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


