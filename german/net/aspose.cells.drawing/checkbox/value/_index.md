---
title: "CheckBox.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBox-Eigenschaft. Gibt an, ob das Kontrollkästchen aktiviert ist oder nicht"
type: docs
url: /de/net/aspose.cells.drawing/checkbox/value/
---
## CheckBox.Value property

Gibt an, ob das Kontrollkästchen aktiviert ist oder nicht.

```csharp
public bool Value { get; set; }
```

### Beispiele

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

### Siehe auch

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


