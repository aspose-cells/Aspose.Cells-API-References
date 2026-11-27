---
title: "CheckBox.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBox-egenskap. Anger om kryssrutan är markerad eller inte"
type: docs
url: /sv/net/aspose.cells.drawing/checkbox/value/
---
## CheckBox.Value property

Indikerar om kryssrutan är markerad eller inte.

```csharp
public bool Value { get; set; }
```

### Exempel

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

### Se även

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


