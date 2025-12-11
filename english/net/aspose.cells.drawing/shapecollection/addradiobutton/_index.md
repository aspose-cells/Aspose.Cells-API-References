---
title: ShapeCollection.AddRadioButton
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a RadioButton to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addradiobutton/
---
## ShapeCollection.AddRadioButton method

Adds a RadioButton to the worksheet.

```csharp
public RadioButton AddRadioButton(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of RadioButton from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of RadioButton from its left column, in unit of pixel. |
| height | Int32 | Represents the height of RadioButton, in unit of pixel. |
| width | Int32 | Represents the width of RadioButton, in unit of pixel. |

### Return Value

A RadioButton object.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRadioButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a radio button to the worksheet
            Aspose.Cells.Drawing.RadioButton radioButton = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 50);
            radioButton.Text = "Option 1";

            // Save the workbook
            workbook.Save("RadioButtonDemo.xlsx");
        }
    }
}
```

### See Also

* class [RadioButton](../../radiobutton/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


