---
title: ShapeCollection.AddButton
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a Button to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addbutton/
---
## ShapeCollection.AddButton method

Adds a Button to the worksheet.

```csharp
public Button AddButton(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Button from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Button from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Button, in unit of pixel. |
| width | Int32 | Represents the width of Button, in unit of pixel. |

### Return Value

A Button object.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a button using the specified parameters
            Aspose.Cells.Drawing.Button button = worksheet.Shapes.AddButton(1, 0, 1, 0, 100, 50);
            button.Text = "Click Me";

            // Save the workbook
            workbook.Save("ButtonDemo.xlsx");
        }
    }
}
```

### See Also

* class [Button](../../button/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


