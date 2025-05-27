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

    public class GradientFillMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape to the worksheet with all required parameters
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);

            try
            {
                // Set fill type to gradient and access the gradient fill
                shape.Fill.Type = FillType.Gradient;

                // Set one color gradient with specified parameters directly through FillFormat
                shape.Fill.SetOneColorGradient(
                    color: Color.Blue,
                    degree: 0.5,
                    style: GradientStyleType.Horizontal,
                    variant: 1
                );

                Console.WriteLine("SetOneColorGradient method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetOneColorGradient: {ex.Message}");
            }

            // Save the workbook to observe the gradient effect
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


