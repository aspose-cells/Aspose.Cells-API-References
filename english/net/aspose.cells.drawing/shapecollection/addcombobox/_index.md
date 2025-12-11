---
title: ShapeCollection.AddComboBox
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a ComboBox to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addcombobox/
---
## ShapeCollection.AddComboBox method

Adds a ComboBox to the worksheet.

```csharp
public ComboBox AddComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of ComboBox from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of ComboBox from its left column, in unit of pixel. |
| height | Int32 | Represents the height of ComboBox, in unit of pixel. |
| width | Int32 | Represents the width of ComboBox, in unit of pixel. |

### Return Value

A ComboBox object.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddComboBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Get the shapes collection
            ShapeCollection shapes = worksheet.Shapes;

            // Add a combo box with specified parameters
            Aspose.Cells.Drawing.ComboBox comboBox = shapes.AddComboBox(1, 0, 1, 0, 100, 50);

            // Add items to the combo box by setting cell values
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Set the input range for the combo box
            comboBox.InputRange = "A1:A3";
            comboBox.DropDownLines = 3;

            // Save the workbook
            workbook.Save("AddComboBoxDemo.xlsx");
        }
    }
}
```

### See Also

* class [ComboBox](../../combobox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


