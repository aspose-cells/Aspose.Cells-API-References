---
title: "CheckBox.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CheckBox. Indica si la casilla de verificación está marcada o no"
type: docs
url: /es/net/aspose.cells.drawing/checkbox/value/
---
## CheckBox.Value property

Indica si el checkbox está marcado o no.

```csharp
public bool Value { get; set; }
```

### Ejemplos

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

### Ver también

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


