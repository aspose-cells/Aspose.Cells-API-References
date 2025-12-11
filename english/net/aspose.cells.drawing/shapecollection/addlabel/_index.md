---
title: ShapeCollection.AddLabel
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a Label to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

Adds a Label to the worksheet.

```csharp
public Label AddLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Label from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Label from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Label, in unit of pixel. |
| width | Int32 | Represents the width of Label, in unit of pixel. |

### Return Value

A Label object.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLabelWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Get the shapes collection
            ShapeCollection shapes = worksheet.Shapes;

            // Add a label to the worksheet
            Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
            label.Text = "Sample Label";

            // Save the workbook
            workbook.Save("AddLabelDemo.xlsx");
        }
    }
}
```

### See Also

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


