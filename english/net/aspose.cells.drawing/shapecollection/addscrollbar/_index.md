---
title: ShapeCollection.AddScrollBar
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a ScrollBar to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addscrollbar/
---
## ShapeCollection.AddScrollBar method

Adds a ScrollBar to the worksheet.

```csharp
public ScrollBar AddScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of ScrollBar from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of ScrollBar from its left column, in unit of pixel. |
| height | Int32 | Represents the height of ScrollBar, in unit of pixel. |
| width | Int32 | Represents the width of ScrollBar, in unit of pixel. |

### Return Value

A ScrollBar object.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddScrollBarWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            ScrollBar scrollBar = shapes.AddScrollBar(1, 0, 100, 20, 0, 100);
            scrollBar.CurrentValue = 50;
            scrollBar.Width = 200;
            scrollBar.Height = 30;

            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### See Also

* class [ScrollBar](../../scrollbar/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


