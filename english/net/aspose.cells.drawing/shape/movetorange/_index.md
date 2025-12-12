---
title: Shape.MoveToRange
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Moves the shape to a specified range
type: docs
url: /net/aspose.cells.drawing/shape/movetorange/
---
## Shape.MoveToRange method

Moves the shape to a specified range.

```csharp
public void MoveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| bottomRow | Int32 | Lower right row index |
| rightColumn | Int32 | Lower right column index |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodMoveToRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to the worksheet
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Move the shape to a specific range
            shape.MoveToRange(12, 3, 13, 5);

            // Save the workbook
            workbook.Save("ShapeMoveToRangeDemo.xlsx");
        }
    }
}
```

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


