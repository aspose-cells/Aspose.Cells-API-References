---
title: GradientFill.SetOneColorGradient
second_title: Aspose.Cells for .NET API Reference
description: GradientFill method. Sets the specified fill to a onecolor gradient. Only applies for Excel 2007
type: docs
url: /net/aspose.cells.drawing/gradientfill/setonecolorgradient/
---
## GradientFill.SetOneColorGradient method

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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to apply gradient fill
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Set the fill type to gradient
                shape.Fill.FillType = FillType.Gradient;

                // Get the gradient fill
                GradientFill gradientFill = shape.Fill.GradientFill;
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Call SetOneColorGradient with realistic parameters
                gradientFill.SetOneColorGradient(
                    Color.Green,        // color
                    0.7,                // degree (70% intensity)
                    GradientStyleType.DiagonalUp,  // style
                    1);                 // variant

                Console.WriteLine("SetOneColorGradient method called successfully with parameters (Green, 0.7, DiagonalUp, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }

            // Save the workbook to demonstrate the effect
            workbook.Save("SetOneColorGradientDemo.xlsx");
        }
    }
}
```

### See Also

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


