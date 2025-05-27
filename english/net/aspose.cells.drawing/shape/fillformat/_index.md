---
title: Shape.FillFormat
second_title: Aspose.Cells for .NET API Reference
description: Shape property. Returns a MsoFillFormat object that contains fill formatting properties for the specified shape
type: docs
url: /net/aspose.cells.drawing/shape/fillformat/
---
## Shape.FillFormat property

Returns a MsoFillFormat object that contains fill formatting properties for the specified shape.

```csharp
[Obsolete("Use Shape.Fill property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoFillFormat FillFormat { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.Fill property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFillFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Set fill format properties
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.Pattern = FillPattern.Solid;
            fillFormat.SolidFill.Color = System.Drawing.Color.Red;
            fillFormat.Transparency = 0.5;

            // Add another shape with gradient fill
            Shape oval = worksheet.Shapes.AddOval(1, 0, 200, 100, 150, 200);
            FillFormat gradientFill = oval.Fill;
            gradientFill.SetTwoColorGradient(
                System.Drawing.Color.Blue,
                System.Drawing.Color.Green,
                GradientStyleType.Horizontal,
                1);

            // Save the workbook
            workbook.Save("ShapeFillFormatDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


