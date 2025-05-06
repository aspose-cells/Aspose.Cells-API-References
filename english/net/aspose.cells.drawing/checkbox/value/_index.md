---
title: CheckBox.Value
second_title: Aspose.Cells for .NET API Reference
description: CheckBox property. Indicates if the checkbox is checked or not
type: docs
url: /net/aspose.cells.drawing/checkbox/value/
---
## CheckBox.Value property

Indicates if the checkbox is checked or not.

```csharp
public bool Value { get; set; }
```

### Examples

```csharp
// Called: checkBox.Value = true; // Check the checkbox
public static void Property_Value()
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
            checkBox.LinkedCell = &quot;A1&quot;; // Link to cell A1
            checkBox.Text = &quot;Accept Terms&quot;; // Set checkbox text
            checkBox.Shadow = false; // No shadow effect

            // Save the workbook
            workbook.Save(&quot;CheckBoxExample.xlsx&quot;);
            workbook.Save(&quot;CheckBoxExample.pdf&quot;);
        }
```

### See Also

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


