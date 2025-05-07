---
title: FillFormat.SetOneColorGradient
second_title: Aspose.Cells for .NET API Reference
description: FillFormat method. Sets the specified fill to a onecolor gradient. Only applies for Excel 2007
type: docs
url: /net/aspose.cells.drawing/fillformat/setonecolorgradient/
---
## FillFormat.SetOneColorGradient method

Sets the specified fill to a one-color gradient. Only applies for Excel 2007.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | One gradient color. |
| degree | Double | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### Examples

```csharp
// Called: chart.NSeries[i].Area.FillFormat.SetOneColorGradient(colorList[i], 0.7, GradientStyleType.FromCenter, 2);
public void Method_Int32_()
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

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


