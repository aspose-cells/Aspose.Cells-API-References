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

            // Add a checkbox to the worksheet
            int index = worksheet.CheckBoxes.Add(5, 5, 100, 20);
            CheckBox checkBox = worksheet.CheckBoxes[index];

            // Display initial CheckValue
            Console.WriteLine("Initial CheckValue: " + checkBox.CheckedValue);

            // Set CheckValue to Checked
            checkBox.CheckedValue = CheckValueType.Checked;
            Console.WriteLine("After setting to Checked: " + checkBox.CheckedValue);

            // Set CheckValue to UnChecked
            checkBox.CheckedValue = CheckValueType.UnChecked;
            Console.WriteLine("After setting to UnChecked: " + checkBox.CheckedValue);

            // Set CheckValue to Mixed
            checkBox.CheckedValue = CheckValueType.Mixed;
            Console.WriteLine("After setting to Mixed: " + checkBox.CheckedValue);

            // Save the workbook
            workbook.Save("CheckBoxPropertyCheckValueDemo.xlsx");
        }
    }
}
```

### See Also

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


