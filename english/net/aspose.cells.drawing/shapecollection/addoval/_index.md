---
title: ShapeCollection.AddOval
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a Oval to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addoval/
---
## ShapeCollection.AddOval method

Adds a Oval to the worksheet.

```csharp
public Oval AddOval(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Oval from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Oval from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Oval, in unit of pixel. |
| width | Int32 | Represents the width of Oval, in unit of pixel. |

### Return Value

A Oval object.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddOvalWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an oval shape to the worksheet
            ShapeCollection shapes = worksheet.Shapes;
            Oval oval = shapes.AddOval(1, 0, 1, 0, 50, 50);

            // Save the workbook
            workbook.Save("AddOvalDemo.xlsx");
        }
    }
}
```

### See Also

* class [Oval](../../oval/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


