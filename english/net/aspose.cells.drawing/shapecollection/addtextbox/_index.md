---
title: ShapeCollection.AddTextBox
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a text box to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

Adds a text box to the worksheet.

```csharp
public TextBox AddTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of textbox from its top row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | Int32 | Represents the height of textbox, in unit of pixel. |
| width | Int32 | Represents the width of textbox, in unit of pixel. |

### Return Value

A [`TextBox`](../../textbox/) object.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Get the shapes collection
            ShapeCollection shapes = worksheet.Shapes;

            // Add a TextBox with specified position and size
            TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
            textBox.Text = "Sample TextBox";

            // Save the workbook
            workbook.Save("TextBoxDemo.xlsx");
        }
    }
}
```

### See Also

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


