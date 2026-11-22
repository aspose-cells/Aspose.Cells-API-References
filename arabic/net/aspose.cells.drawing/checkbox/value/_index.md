---
title: "CheckBox.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CheckBox. تشير إلى ما إذا كان مربع الاختيار محددًا أم لا"
type: docs
url: /ar/net/aspose.cells.drawing/checkbox/value/
---
## CheckBox.Value property

يشير إلى ما إذا كانت خانة الاختيار محددة أم لا.

```csharp
public bool Value { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


