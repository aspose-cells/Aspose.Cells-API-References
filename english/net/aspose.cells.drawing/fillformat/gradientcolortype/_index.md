---
title: FillFormat.GradientColorType
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient color type for the specified fill
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientcolortype/
---
## FillFormat.GradientColorType property

Returns the gradient color type for the specified fill.

```csharp
public GradientColorType GradientColorType { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyGradientColorTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to demonstrate gradient fill
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            try
            {
                // Set a two-color gradient fill
                shape.Fill.SetTwoColorGradient(Color.Red, Color.Blue,
                    GradientStyleType.Horizontal, 2);

                // Access the FillFormat to get GradientColorType
                FillFormat fillFormat = shape.Fill;

                // Display the GradientColorType value
                Console.WriteLine("GradientColorType: " + fillFormat.GradientColorType);

                // Save the workbook
                workbook.Save("GradientColorTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [GradientColorType](../../gradientcolortype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


