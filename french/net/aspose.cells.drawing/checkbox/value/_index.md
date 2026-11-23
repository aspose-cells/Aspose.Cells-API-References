---
title: "CheckBox.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CheckBox. Indique si la case à cocher est cochée ou non"
type: docs
url: /fr/net/aspose.cells.drawing/checkbox/value/
---
## CheckBox.Value property

Indique si la case à cocher est cochée ou non.

```csharp
public bool Value { get; set; }
```

### Exemples

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

### Voir aussi

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


