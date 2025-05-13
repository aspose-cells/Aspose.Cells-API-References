---
title: FillFormat.SetTwoColorGradient
second_title: Aspose.Cells for .NET API Reference
description: FillFormat method. Sets the specified fill to a twocolor gradient. Only applies for Excel 2007
type: docs
url: /net/aspose.cells.drawing/fillformat/settwocolorgradient/
---
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}

Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| color2 | Color | Two gradient color. |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### Examples

```csharp
// Called: fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);
public static void FillFormat_Method_SetTwoColorGradient()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Access the chart's plot area
            PlotArea plotArea = chart.PlotArea;

            // Access the fill format of the plot area
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // Set a two-color gradient fill with a specific direction
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Output the gradient direction type
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Save the workbook
            workbook.Save("GradientDirectionTypeExample.xlsx");
            workbook.Save("GradientDirectionTypeExample.pdf");
        }
```

### See Also

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}

Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2, 
    double transparency2, GradientStyleType style, int variant)
```

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| transparency1 | Double | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | Color | Two gradient color. |
| transparency2 | Double | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### See Also

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


