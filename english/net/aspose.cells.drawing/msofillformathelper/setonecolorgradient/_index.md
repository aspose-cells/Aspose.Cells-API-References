---
title: MsoFillFormatHelper.SetOneColorGradient
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper method. Sets the specified fill to a onecolor gradient
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/setonecolorgradient/
---
## MsoFillFormatHelper.SetOneColorGradient method

Sets the specified fill to a one-color gradient.

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

    public class MsoFillFormatHelperMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a rectangle shape to apply gradient fill
            Shape rectangle = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 100, 200);

            try
            {
                // Get MsoFillFormat from shape's fill format
                MsoFillFormat fillFormat = rectangle.FillFormat;

                // Apply one-color gradient with specified parameters
                fillFormat.SetOneColorGradient(
                    color: Color.Blue,
                    degree: 0.5,
                    style: GradientStyleType.Horizontal,
                    variant: 2
                );

                Console.WriteLine("Method executed successfully with parameters (Color, Double, GradientStyleType, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetOneColorGradient method: {ex.Message}");
            }

            // Save the modified workbook
            workbook.Save("MethodSetOneColorGradientDemo.xlsx");
        }
    }
}
```

### See Also

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


