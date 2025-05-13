---
title: Worksheet.CheckBoxes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets a CheckBox collection
type: docs
url: /net/aspose.cells/worksheet/checkboxes/
---
## Worksheet.CheckBoxes property

Gets a [`CheckBox`](../../../aspose.cells.drawing/checkbox/) collection.

```csharp
public CheckBoxCollection CheckBoxes { get; }
```

### Examples

```csharp
// Called: int index = sheet.CheckBoxes.Add(15, 15, 20, 100);
public static void Worksheet_Property_CheckBoxes()
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

* class [CheckBoxCollection](../../../aspose.cells.drawing/checkboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


