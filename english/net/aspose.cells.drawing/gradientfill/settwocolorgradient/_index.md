---
title: GradientFill.SetTwoColorGradient
second_title: Aspose.Cells for .NET API Reference
description: GradientFill method. Sets the specified fill to a twocolor gradient. Only applies for Excel 2007
type: docs
url: /net/aspose.cells.drawing/gradientfill/settwocolorgradient/
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Gradient Fill Demo");

            try
            {
                Style cellStyle = cell.GetStyle();
                
                cellStyle.SetTwoColorGradient(
                    Color.LightSkyBlue,
                    Color.DarkBlue,
                    GradientStyleType.Horizontal,
                    2
                );
                
                cell.SetStyle(cellStyle);
                Console.WriteLine("Two-color gradient applied successfully to cell A1.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying gradient: {ex.Message}");
            }

            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### See Also

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
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

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetTwoColorGradientWithColorDoubleColorDoubleGradientDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create a cell and set value to visualize gradient effect
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Two Color Gradient Demo");
            
            // Create a custom style
            Style style = workbook.CreateStyle();

            try
            {
                // Create colors with transparency using alpha channel
                Color color1 = Color.FromArgb((int)((1 - 0.3) * 255), Color.LightBlue);
                Color color2 = Color.FromArgb((int)((1 - 0.7) * 255), Color.DarkBlue);
                
                // Set two color gradient directly through Style's method
                style.SetTwoColorGradient(
                    color1: color1,
                    color2: color2,
                    gradientStyleType: GradientStyleType.Horizontal,
                    variant: 1
                );

                // Apply style to cell
                cell.SetStyle(style);
                
                // Adjust row height and column width for better visibility
                worksheet.Cells.SetRowHeight(0, 30);
                worksheet.Cells.SetColumnWidth(0, 20);
                
                Console.WriteLine("Gradient applied successfully with parameters: (Color, Double, Color, Double, GradientStyleType, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTwoColorGradient method: {ex.Message}");
            }
            
            // Save the workbook
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### See Also

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


