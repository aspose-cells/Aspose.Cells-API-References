---
title: PatternFill.BackgroundCellsColor
second_title: Aspose.Cells for .NET API Reference
description: PatternFill property. Gets and sets the foreground CellsColor object
type: docs
url: /net/aspose.cells.drawing/patternfill/backgroundcellscolor/
---
## PatternFill.BackgroundCellsColor property

Gets and sets the foreground [`CellsColor`](../../../aspose.cells/cellscolor/) object.

```csharp
public CellsColor BackgroundCellsColor { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackgroundCellsColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape to demonstrate pattern fill
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            try
            {
                // Set fill type to pattern
                shape.Fill.FillType = FillType.Pattern;

                // Get the PatternFill instance
                PatternFill patternFill = shape.Fill.PatternFill;

                // Set pattern type and colors
                patternFill.Pattern = FillPattern.WideDownwardDiagonal;
                patternFill.ForegroundColor = Color.Red;
                patternFill.BackgroundColor = Color.Yellow;

                // Access and modify BackgroundCellsColor properties
                patternFill.BackgroundCellsColor.Color = Color.Blue;
                patternFill.BackgroundCellsColor.Argb = Color.Blue.ToArgb();
                patternFill.BackgroundCellsColor.Transparency = 0.3;

                // Display the BackgroundCellsColor properties
                Console.WriteLine("BackgroundCellsColor Type: " + patternFill.BackgroundCellsColor.Type);
                Console.WriteLine("BackgroundCellsColor Color: " + patternFill.BackgroundCellsColor.Color);
                Console.WriteLine("BackgroundCellsColor ARGB: " + patternFill.BackgroundCellsColor.Argb);
                Console.WriteLine("BackgroundCellsColor Transparency: " + patternFill.BackgroundCellsColor.Transparency);

                // Save the workbook
                workbook.Save("BackgroundCellsColorDemo.xlsx");
                Console.WriteLine("BackgroundCellsColor demonstration completed successfully.");
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
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


