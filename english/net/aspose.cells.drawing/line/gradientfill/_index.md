---
title: Line.GradientFill
second_title: Aspose.Cells for .NET API Reference
description: Line property. Represents gradient fill
type: docs
url: /net/aspose.cells.drawing/line/gradientfill/
---
## Line.GradientFill property

Represents gradient fill.

```csharp
public GradientFill GradientFill { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.LinePropertyGradientFillDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class LinePropertyGradientFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a rectangle shape with visible borders
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            LineFormat line = shape.Line; // Changed type from Line to LineFormat

            // Display initial gradient fill properties
            Console.WriteLine("Initial Gradient Fill Type: " + line.GradientFill.FillType);

            // Configure two-color gradient for the line
            line.GradientFill.SetTwoColorGradient(
                Color.Red, 0.0, 
                Color.Blue, 0.0, 
                GradientStyleType.Horizontal, 
                1
            );
            line.GradientFill.Angle = 45;

            // Add another shape to demonstrate different settings
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 200, 1, 0, 100, 150);
            shape2.Line.GradientFill.SetOneColorGradient(
                Color.Green, 0.5, 
                GradientStyleType.Vertical, 
                2
            );

            // Save modified workbook
            workbook.Save("LinePropertyGradientFillDemo.xlsx");
        }
    }
}
```

### See Also

* class [GradientFill](../../gradientfill/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


