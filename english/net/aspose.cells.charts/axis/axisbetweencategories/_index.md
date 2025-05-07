---
title: Axis.AxisBetweenCategories
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents if the value axis crosses the category axis between categories
type: docs
url: /net/aspose.cells.charts/axis/axisbetweencategories/
---
## Axis.AxisBetweenCategories property

Represents if the value axis crosses the category axis between categories.

```csharp
public bool AxisBetweenCategories { get; set; }
```

### Remarks

This property applies only to category axes, and it doesn't apply to 3-D charts.

### Examples

```csharp
// Called: categoryAxis.AxisBetweenCategories = false;
public void Property_AxisBetweenCategories()
        {
            Workbook workbook = new Workbook(Path.Combine(path, "TEST_Data.xlsx"));

            Worksheet datasheet = workbook.Worksheets[0];
            datasheet.Name = "Data";
            datasheet.IsGridlinesVisible = true;

            int sheetIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartsheet = workbook.Worksheets[sheetIndex];
            chartsheet.Name = "Chart";
            chartsheet.IsGridlinesVisible = false;

            int chartIndex = chartsheet.Charts.Add(ChartType.AreaStacked, 1, 1, 1, 1);
            Chart chart = chartsheet.Charts[chartIndex];
            chart.PlotArea.Border.IsVisible = true;
            chart.PlotArea.Area.ForegroundColor = Color.Transparent;
            chart.PageSetup.Orientation = PageOrientationType.Landscape;
            chart.Legend.Position = LegendPositionType.Top;

            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.AxisBetweenCategories = false;
            categoryAxis.CategoryType = CategoryType.AutomaticScale;
            categoryAxis.MajorTickMark = TickMarkType.Outside;
            categoryAxis.MajorUnitScale = TimeUnit.Days;
            categoryAxis.MinorGridLines.IsVisible = false;
            categoryAxis.TickLabels.NumberFormat = "General";
            categoryAxis.TickLabels.RotationAngle = 45;
            categoryAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;
            categoryAxis.TickLabelSpacing = 2;

            chart.ValueAxis.MajorGridLines.IsVisible = false;
            chart.ValueAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            chart.NSeries.Add("Data!B2:H49", true);
            chart.NSeries.CategoryData = "Data!A2:A49";

            Color[] colorList = {   Color.FromArgb(0, 128, 0), 
                            Color.FromArgb(255, 11, 11), 
                            Color.FromArgb(255, 206, 45), 
                            Color.FromArgb(16, 16, 129), 
                            Color.FromArgb(156, 156, 156), 
                            Color.FromArgb(0, 0, 0), 
                            Color.FromArgb(18, 205, 255), 
                            Color.FromArgb(255, 55, 55), 
                            Color.FromArgb(128, 255, 255), 
                            Color.FromArgb(128, 0, 128), 
                            Color.FromArgb(255, 255, 128), 
                            Color.FromArgb(192, 192, 192) };

            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                chart.NSeries[i].Name = cells[0, i + 1].Value.ToString();
                chart.NSeries[i].Area.FillFormat.SetOneColorGradient(colorList[i], 0.7, GradientStyleType.FromCenter, 2);
            }

            string fileName = Path.Combine(Constants.destPath, "TEST_Data_Chart_out.xls");
            if (File.Exists(fileName))
            {
                File.Delete(fileName);
            }

            //workbook.Save(fileName, FileFormatType.Excel2007Xlsx);
            workbook.Save(fileName);

        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


