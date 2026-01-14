---
title: PatternFill.ForeTransparency
second_title: Aspose.Cells for .NET API Reference
description: PatternFill property. Gets or sets the transparency of foreground color
type: docs
url: /net/aspose.cells.drawing/patternfill/foretransparency/
---
## PatternFill.ForeTransparency property

Gets or sets the transparency of foreground color.

```csharp
public double ForeTransparency { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForeTransparencyDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape to demonstrate pattern fill
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Set fill type to pattern
            shape.Fill.FillType = FillType.Pattern;

            // Get the PatternFill instance
            PatternFill patternFill = shape.Fill.PatternFill;

            // Configure pattern fill properties
            patternFill.Pattern = FillPattern.Solid;
            patternFill.ForegroundColor = Color.Red;
            patternFill.BackgroundColor = Color.Blue;

            try
            {
                // Display initial ForeTransparency value
                Console.WriteLine("Initial ForeTransparency value: " + patternFill.ForeTransparency);

                // Set new ForeTransparency value (50% transparency)
                patternFill.ForeTransparency = 0.5;

                // Display updated ForeTransparency value
                Console.WriteLine("Updated ForeTransparency value: " + patternFill.ForeTransparency);

                // Save the workbook
                workbook.Save("ForeTransparencyDemo.xlsx");
                Console.WriteLine("ForeTransparency demonstration completed successfully.");
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

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


