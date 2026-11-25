---
title: "CheckBox.Shadow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CheckBox. Indica se la casella combinata ha ombreggiatura 3D"
type: docs
url: /it/net/aspose.cells.drawing/checkbox/shadow/
---
## CheckBox.Shadow property

Indica se la combobox ha ombreggiatura 3D.

```csharp
public bool Shadow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi una casella di controllo al foglio di lavoro e ottieni il suo indice
            int checkBoxIndex = sheet.CheckBoxes.Add(1, 1, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
            
            // Configura le proprietà della casella di controllo
            checkBox.Text = "Enable Feature";
            checkBox.Value = true;
            
            // Dimostra la proprietà Shadow
            checkBox.Shadow = true; // Enable shadow effect
            workbook.Save("CheckBoxWithShadow.xlsx");
            
            checkBox.Shadow = false; // Disable shadow effect
            workbook.Save("CheckBoxWithoutShadow.xlsx");
        }
    }
}
```

### Vedi anche

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


