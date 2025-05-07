---
title: CheckBoxCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: CheckBoxCollection method. Adds a checkBox to the collection
type: docs
url: /net/aspose.cells.drawing/checkboxcollection/add/
---
## CheckBoxCollection.Add method

Adds a checkBox to the collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| height | Int32 | Height of checkBox, in unit of pixel. |
| width | Int32 | Width of checkBox, in unit of pixel. |

### Return Value

[`CheckBox`](../../checkbox/) object index.

### Examples

```csharp
// Called: int index = sheet.CheckBoxes.Add(15, 15, 20, 100);
public static void Method_Int32_()
        {
            // Create a new Workbook.
            Workbook workbook = new Workbook();

            // Get the first worksheet in the workbook.
            Worksheet sheet = workbook.Worksheets[0];

            // Add a CheckBox to the worksheet.
            int index = sheet.CheckBoxes.Add(15, 15, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[index];
            checkBox.Text = "Check Box 1";

            // Save the workbook.
            workbook.Save("CheckBoxCollectionExample.xlsx");
            workbook.Save("CheckBoxCollectionExample.pdf");
            return;
        }
```

### See Also

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


