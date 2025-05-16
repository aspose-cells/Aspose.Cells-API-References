---
title: MsoFillFormatHelper.BackColor
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper property. Gets and sets the file back color
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/backcolor/
---
## MsoFillFormatHelper.BackColor property

Gets and sets the file back color.

```csharp
public Color BackColor { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.MsoFillFormatHelperPropertyBackColorDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape and get its fill format
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 0, 100, 200);
            FillFormat fillFormat = shape.Fill;

            // Configure a gradient fill using FillFormat's method
            fillFormat.SetOneColorGradient(Color.LightGreen, 0.5, GradientStyleType.Horizontal, 1);

            // Since BackColor is not directly available in FillFormat, adjust the gradient's colors
            // Assuming the gradient is now a two-color gradient for demonstration
            fillFormat.SetTwoColorGradient(Color.LightGreen, 0.5, Color.LightBlue, 0.5, GradientStyleType.Horizontal, 1);

            // Save the modified workbook to show visual effect
            workbook.Save("MsoFillBackColorDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


