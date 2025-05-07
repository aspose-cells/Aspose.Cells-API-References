---
title: CheckBox.Shadow
second_title: Aspose.Cells for .NET API Reference
description: CheckBox property. Indicates whether the combobox has 3D shading
type: docs
url: /net/aspose.cells.drawing/checkbox/shadow/
---
## CheckBox.Shadow property

Indicates whether the combobox has 3-D shading.

```csharp
public bool Shadow { get; set; }
```

### Examples

```csharp
// Called: checkBox.Shadow = false; // No shadow effect
public static void Property_Shadow()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add a checkbox to the worksheet
            CheckBoxCollection checkBoxes = sheet.CheckBoxes;
            int upperLeftRow = 0;
            int upperLeftColumn = 0;
            int height = 20;
            int width = 100;

            // Add a checkbox at specified position
            int checkBoxIndex = checkBoxes.Add(upperLeftRow, upperLeftColumn, height, width);
            CheckBox checkBox = checkBoxes[checkBoxIndex];

            // Set properties for the checkbox
            checkBox.Value = true; // Check the checkbox
            checkBox.LinkedCell = "A1"; // Link to cell A1
            checkBox.Text = "Accept Terms"; // Set checkbox text
            checkBox.Shadow = false; // No shadow effect

            // Save the workbook
            workbook.Save("CheckBoxExample.xlsx");
            workbook.Save("CheckBoxExample.pdf");
        }
```

### See Also

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


