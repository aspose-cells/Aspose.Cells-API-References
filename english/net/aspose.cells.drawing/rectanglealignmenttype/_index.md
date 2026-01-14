---
title: Enum RectangleAlignmentType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.RectangleAlignmentType enum. Represents how to position two rectangles relative to each other
type: docs
url: /net/aspose.cells.drawing/rectanglealignmenttype/
---
## RectangleAlignmentType enumeration

Represents how to position two rectangles relative to each other.

```csharp
public enum RectangleAlignmentType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Bottom | `0` | Bottom |
| BottomLeft | `1` | BottomLeft |
| BottomRight | `2` | BottomRight |
| Center | `3` | Center |
| Left | `4` | Left |
| Right | `5` | Right |
| Top | `6` | Top |
| TopLeft | `7` | TopLeft |
| TopRight | `8` | TopRight |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassRectangleAlignmentTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a rectangle shape to demonstrate alignment
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 200, 100, 100);

                // Demonstrate different alignment types
                Console.WriteLine("Available RectangleAlignmentType values:");
                Console.WriteLine("Bottom: " + RectangleAlignmentType.Bottom);
                Console.WriteLine("BottomLeft: " + RectangleAlignmentType.BottomLeft);
                Console.WriteLine("BottomRight: " + RectangleAlignmentType.BottomRight);
                Console.WriteLine("Center: " + RectangleAlignmentType.Center);
                Console.WriteLine("Left: " + RectangleAlignmentType.Left);
                Console.WriteLine("Right: " + RectangleAlignmentType.Right);
                Console.WriteLine("Top: " + RectangleAlignmentType.Top);
                Console.WriteLine("TopLeft: " + RectangleAlignmentType.TopLeft);
                Console.WriteLine("TopRight: " + RectangleAlignmentType.TopRight);

                // Set alignment based on one of the enum values
                rectangle.TextHorizontalAlignment = TextAlignmentType.Center;
                rectangle.TextVerticalAlignment = TextAlignmentType.Center;

                // Save the workbook
                workbook.Save("RectangleAlignmentTypeDemo.xlsx");
                Console.WriteLine("RectangleAlignmentType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating RectangleAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


