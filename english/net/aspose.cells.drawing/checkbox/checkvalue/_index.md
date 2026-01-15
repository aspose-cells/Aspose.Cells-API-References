---
title: CheckBox.CheckValue
second_title: Aspose.Cells for .NET API Reference
description: CheckBox property. Gets or set checkbox value
type: docs
url: /net/aspose.cells.drawing/checkbox/checkvalue/
---
## CheckBox.CheckValue property

Gets or set checkbox' value.

```csharp
[Obsolete("Use CheckBox.CheckValueType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CheckValueType CheckValue { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use CheckBox.CheckValueType property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CheckBoxPropertyCheckValueDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a checkbox to the worksheet
                int checkBoxIndex = worksheet.CheckBoxes.Add(1, 1, 20, 100);
                CheckBox checkBox = worksheet.CheckBoxes[checkBoxIndex];

                // Set initial properties
                checkBox.Text = "Sample Checkbox";
                checkBox.Value = true;

                // Display the current CheckValue
                Console.WriteLine("Initial CheckValue: " + checkBox.CheckValue);

                // Set CheckValue to a different state
                checkBox.CheckValue = CheckValueType.Mixed;
                Console.WriteLine("Updated CheckValue: " + checkBox.CheckValue);

                // Save the workbook
                workbook.Save("CheckBoxCheckValueDemo.xlsx");

                // Load the saved workbook to verify
                Workbook loadedWorkbook = new Workbook("CheckBoxCheckValueDemo.xlsx");
                CheckBox loadedCheckBox = (CheckBox)loadedWorkbook.Worksheets[0].Shapes[0];
                Console.WriteLine("Loaded CheckValue: " + loadedCheckBox.CheckValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


