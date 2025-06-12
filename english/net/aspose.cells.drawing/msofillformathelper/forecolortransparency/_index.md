---
title: MsoFillFormatHelper.ForeColorTransparency
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper property. Returns or sets the degree of fore color of the specified fill as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/forecolortransparency/
---
## MsoFillFormatHelper.ForeColorTransparency property

Returns or sets the degree of fore color of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double ForeColorTransparency { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyForeColorTransparencyDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape to access fill formatting
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 1, 1, 200, 100);
            MsoFillFormat fillFormat = shape.FillFormat;

            // Set solid fill color (blue) with initial transparency
            fillFormat.ForeColor = Color.Blue;
            Console.WriteLine("Initial ForeColorTransparency: " + fillFormat.Transparency);

            // Make fill semi-transparent (50% opacity)
            fillFormat.Transparency = 0.5;
            Console.WriteLine("Modified ForeColorTransparency: " + fillFormat.Transparency);

            // Add another shape with different transparency for comparison
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 150, 1, 1, 200, 100);
            shape2.FillFormat.ForeColor = Color.Red;
            shape2.FillFormat.Transparency = 0.8;

            // Save the workbook to demonstrate visual effects
            workbook.Save("ForeColorTransparencyDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


