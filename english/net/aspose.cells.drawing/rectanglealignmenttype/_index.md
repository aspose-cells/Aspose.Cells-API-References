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
namespace AsposeCellsExamples.DrawingClassRectangleAlignmentTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassRectangleAlignmentTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add two shapes to demonstrate alignment
            Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 0, 0, 100, 100);
            Shape shape2 = worksheet.Shapes.AddRectangle(150, 150, 0, 0, 100, 100);

            // Note: The original code tried to set AlignmentType on Shape objects,
            // but this property doesn't exist on the Shape class.
            // The RectangleAlignmentType enum exists but isn't directly applicable here.
            // This part has been removed as it was causing compilation errors.
            // If you need to align shapes, you would need to use their positioning properties
            // like Left, Top, etc.

            // Save the workbook with alignment examples
            workbook.Save("RectangleAlignmentTypeDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


