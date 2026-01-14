---
title: Class GradientStop
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.GradientStop class. Represents the gradient stop
type: docs
url: /net/aspose.cells.drawing/gradientstop/
---
## GradientStop class

Represents the gradient stop.

```csharp
public class GradientStop
```

## Properties

| Name | Description |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/gradientstop/cellscolor/) { get; } | Gets the color of this gradient stop. |
| [Position](../../aspose.cells.drawing/gradientstop/position/) { get; set; } | The position of the stop. |
| [Transparency](../../aspose.cells.drawing/gradientstop/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassGradientStopDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a shape with gradient fill
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
                shape.Fill.FillType = FillType.Gradient;
                GradientFill gradientFill = shape.Fill.GradientFill;
                gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

                // Create color for gradient stop
                CellsColor color = workbook.CreateCellsColor();
                color.Color = Color.Blue;

                // Add gradient stop
                gradientFill.GradientStops.Add(0, color, 30);

                // Access the gradient stop
                GradientStop stop = gradientFill.GradientStops[0];

                // Demonstrate basic functionality
                Console.WriteLine("GradientStop instance created successfully");
                Console.WriteLine("Position: " + stop.Position);
                Console.WriteLine("Transparency: " + stop.Transparency);
                Console.WriteLine("CellsColor Type: " + stop.CellsColor.Type);

                // Modify properties
                stop.Position = 0.5;
                stop.Transparency = 0.7;

                Console.WriteLine("Modified Position: " + stop.Position);
                Console.WriteLine("Modified Transparency: " + stop.Transparency);

                // Save the workbook
                workbook.Save("GradientStopDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientStop: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


