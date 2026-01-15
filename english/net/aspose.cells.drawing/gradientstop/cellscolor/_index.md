---
title: GradientStop.CellsColor
second_title: Aspose.Cells for .NET API Reference
description: GradientStop property. Gets the color of this gradient stop
type: docs
url: /net/aspose.cells.drawing/gradientstop/cellscolor/
---
## GradientStop.CellsColor property

Gets the color of this gradient stop.

```csharp
public CellsColor CellsColor { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyCellsColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
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

                // Access the gradient stop and display its CellsColor properties
                GradientStop stop = gradientFill.GradientStops[0];
                CellsColor stopColor = stop.CellsColor;

                Console.WriteLine("Gradient Stop CellsColor Properties:");
                Console.WriteLine("Color Type: " + stopColor.Type);
                Console.WriteLine("RGB Color: " + stopColor.Color);
                Console.WriteLine("ARGB Value: " + stopColor.Argb);
                Console.WriteLine("Transparency: " + stopColor.Transparency);

                // Save the workbook
                workbook.Save("GradientStopCellsColorDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


