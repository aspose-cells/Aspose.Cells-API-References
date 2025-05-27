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
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int checkBoxIndex = sheet.CheckBoxes.Add(0, 0, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
            checkBox.Value = true;
            checkBox.Text = "Sample Checkbox";

            workbook.Save("CheckBoxValueDemo.xlsx");
        }
    }
}
```

### See Also

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


