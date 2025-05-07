---
title: SeriesLayoutProperties.ShowMeanLine
second_title: Aspose.Cells for .NET API Reference
description: SeriesLayoutProperties property. Indicates whether showing the line connecting all mean points
type: docs
url: /net/aspose.cells.charts/serieslayoutproperties/showmeanline/
---
## SeriesLayoutProperties.ShowMeanLine property

Indicates whether showing the line connecting all mean points.

```csharp
public bool ShowMeanLine { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[series_index].LayoutProperties.ShowMeanLine = false;
[Test]
        public void Property_ShowMeanLine()
        {
            var index = 0;
            var sheetName = "BoxwhiskerChart";
            string excelTemplateRelativePath = Constants.sourcePath + @"CELLSNET46568.xlsx";
            var templatePath = excelTemplateRelativePath;
            var excel = new Workbook(templatePath);
            excel.Worksheets.AddCopy(index);
            var sheet = excel.Worksheets[index];
            var datacell = sheet.Cells["A" + 1];
            datacell.PutValue("");
            for (int i = 2; i <= 6; i++)
            {
                datacell = sheet.Cells["A" + i];
                datacell.PutValue("19-Jan");
            }
            for (int i = 7; i <= 11; i++)
            {
                datacell = sheet.Cells["A" + i];
                datacell.PutValue("1-Feb");
            }

            sheet.Cells["B1"].PutValue("Team A");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(150);
            sheet.Cells["B4"].PutValue(300);
            sheet.Cells["B5"].PutValue(400);
            sheet.Cells["B6"].PutValue(500);
            sheet.Cells["B7"].PutValue(50);
            sheet.Cells["B8"].PutValue(150);
            sheet.Cells["B9"].PutValue(300);
            sheet.Cells["B10"].PutValue(400);
            sheet.Cells["B11"].PutValue(500);

            sheet.Cells["C1"].PutValue("Team B");
            sheet.Cells["C2"].PutValue(50);
            sheet.Cells["C3"].PutValue(150);
            sheet.Cells["C4"].PutValue(300);
            sheet.Cells["C5"].PutValue(400);
            sheet.Cells["C6"].PutValue(500);
            sheet.Cells["C7"].PutValue(50);
            sheet.Cells["C8"].PutValue(150);
            sheet.Cells["C9"].PutValue(300);
            sheet.Cells["C10"].PutValue(400);
            sheet.Cells["C11"].PutValue(500);
            var chartArea = "B" + 2 + ":" + "C" + 11;

            var categoryData = "A" + 2 + ":A" + 11;
            int index1 = sheet.Charts.Add(ChartType.BoxWhisker, 0, 3, 0 + 20, 10);

            var chart = sheet.Charts[index1];
            chart.SetChartDataRange(chartArea, true);
            chart.NSeries.CategoryData = categoryData;
            var seriesName = new List<string> { "Team 1", "Team 2" };
            var seriesTheme = new List<ThemeColorType> { ThemeColorType.Accent1, ThemeColorType.Accent2 };
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

            excel.Save(Constants.destPath + "CELLSNET46568.xlsx");
        }
```

### See Also

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


