---
title: SeriesLayoutProperties.ShowInnerPoints
second_title: Aspose.Cells for .NET API Reference
description: SeriesLayoutProperties property. Indicates whether showing nonoutlier data points
type: docs
url: /net/aspose.cells.charts/serieslayoutproperties/showinnerpoints/
---
## SeriesLayoutProperties.ShowInnerPoints property

Indicates whether showing non-outlier data points.

```csharp
public bool ShowInnerPoints { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[series_index].LayoutProperties.ShowInnerPoints = false;
[Test]
        public void Property_ShowInnerPoints()
        {
            var index = 0;
            var sheetName = &quot;BoxwhiskerChart&quot;;
            string excelTemplateRelativePath = Constants.sourcePath + @&quot;CELLSNET46568.xlsx&quot;;
            var templatePath = excelTemplateRelativePath;
            var excel = new Workbook(templatePath);
            excel.Worksheets.AddCopy(index);
            var sheet = excel.Worksheets[index];
            var datacell = sheet.Cells[&quot;A&quot; + 1];
            datacell.PutValue(&quot;&quot;);
            for (int i = 2; i &lt;= 6; i++)
            {
                datacell = sheet.Cells[&quot;A&quot; + i];
                datacell.PutValue(&quot;19-Jan&quot;);
            }
            for (int i = 7; i &lt;= 11; i++)
            {
                datacell = sheet.Cells[&quot;A&quot; + i];
                datacell.PutValue(&quot;1-Feb&quot;);
            }

            sheet.Cells[&quot;B1&quot;].PutValue(&quot;Team A&quot;);
            sheet.Cells[&quot;B2&quot;].PutValue(50);
            sheet.Cells[&quot;B3&quot;].PutValue(150);
            sheet.Cells[&quot;B4&quot;].PutValue(300);
            sheet.Cells[&quot;B5&quot;].PutValue(400);
            sheet.Cells[&quot;B6&quot;].PutValue(500);
            sheet.Cells[&quot;B7&quot;].PutValue(50);
            sheet.Cells[&quot;B8&quot;].PutValue(150);
            sheet.Cells[&quot;B9&quot;].PutValue(300);
            sheet.Cells[&quot;B10&quot;].PutValue(400);
            sheet.Cells[&quot;B11&quot;].PutValue(500);

            sheet.Cells[&quot;C1&quot;].PutValue(&quot;Team B&quot;);
            sheet.Cells[&quot;C2&quot;].PutValue(50);
            sheet.Cells[&quot;C3&quot;].PutValue(150);
            sheet.Cells[&quot;C4&quot;].PutValue(300);
            sheet.Cells[&quot;C5&quot;].PutValue(400);
            sheet.Cells[&quot;C6&quot;].PutValue(500);
            sheet.Cells[&quot;C7&quot;].PutValue(50);
            sheet.Cells[&quot;C8&quot;].PutValue(150);
            sheet.Cells[&quot;C9&quot;].PutValue(300);
            sheet.Cells[&quot;C10&quot;].PutValue(400);
            sheet.Cells[&quot;C11&quot;].PutValue(500);
            var chartArea = &quot;B&quot; + 2 + &quot;:&quot; + &quot;C&quot; + 11;

            var categoryData = &quot;A&quot; + 2 + &quot;:A&quot; + 11;
            int index1 = sheet.Charts.Add(ChartType.BoxWhisker, 0, 3, 0 + 20, 10);

            var chart = sheet.Charts[index1];
            chart.SetChartDataRange(chartArea, true);
            chart.NSeries.CategoryData = categoryData;
            var seriesName = new List&lt;string&gt; { &quot;Team 1&quot;, &quot;Team 2&quot; };
            var seriesTheme = new List&lt;ThemeColorType&gt; { ThemeColorType.Accent1, ThemeColorType.Accent2 };
            int series_index = 0;
            foreach (var series in seriesName)
            {
                chart.NSeries[series_index].Name = series;
                chart.NSeries[series_index].LayoutProperties.ShowMeanLine = false;
                chart.NSeries[series_index].LayoutProperties.ShowInnerPoints = false;
                chart.NSeries[series_index].Area.FillFormat.FillType = FillType.None;
                chart.NSeries[series_index].Border.FormattingType = ChartLineFormattingType.Solid;
                chart.NSeries[series_index].Border.Style = LineType.Solid;
                chart.NSeries[series_index].Border.ThemeColor = new ThemeColor(seriesTheme[series_index], 0);
                series_index++;
            }

            excel.Save(Constants.destPath + &quot;CELLSNET46568.xlsx&quot;);
        }
```

### See Also

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


