---
title: Series.LegendEntry
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the legend entry according to this series
type: docs
url: /net/aspose.cells.charts/series/legendentry/
---
## Series.LegendEntry property

Gets the legend entry according to this series.

```csharp
public LegendEntry LegendEntry { get; }
```

### Examples

```csharp
// Called: chart.NSeries[index].LegendEntry.IsDeleted = true;
[Test]
        public void Property_LegendEntry()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET44073/&quot;;
            var workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[&quot;K1&quot;].PutValue(50);
            worksheet.Cells[&quot;K2&quot;].PutValue(120);
            worksheet.Cells[&quot;K3&quot;].PutValue(160);
            worksheet.Cells[&quot;K4&quot;].PutValue(200);

            worksheet.Cells[&quot;L1&quot;].PutValue(4);
            worksheet.Cells[&quot;L2&quot;].PutValue(20);
            worksheet.Cells[&quot;L3&quot;].PutValue(40);
            worksheet.Cells[&quot;L4&quot;].PutValue(120);

            worksheet.Cells.Columns[10].IsHidden = true;
            worksheet.Cells.Columns[11].IsHidden = true;

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 0, 0, 20, 7);

            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            chart.PlotVisibleCells = false;
            int index = chart.NSeries.Add(&quot;K1:K4&quot;, true);
            chart.NSeries[index].LegendEntry.IsDeleted = true;
            chart.NSeries.Add(&quot;L1:L4&quot;, true);

            var htmlSaveOptions = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
                ImageOptions =
                {
                    ImageType = ImageType.Png
                }
            };
            workbook.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;);
            workbook.Save(CreateFolder(filePath) + &quot;out.html&quot;, htmlSaveOptions);
        }
```

### See Also

* class [LegendEntry](../../legendentry/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


