---
title: "CheckBox.Shadow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBox-Eigenschaft. Gibt an, ob das Kombinationsfeld 3D-Schattierung hat"
type: docs
url: /de/net/aspose.cells.drawing/checkbox/shadow/
---
## CheckBox.Shadow property

Gibt an, ob die ComboBox 3‑D‑Schattierung hat.

```csharp
public bool Shadow { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie ein Kontrollkästchen zum Arbeitsblatt hinzu und erhalten Sie dessen Index
            int checkBoxIndex = sheet.CheckBoxes.Add(1, 1, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
            
            // Kontrollkästchen-Eigenschaften konfigurieren
            checkBox.Text = "Enable Feature";
            checkBox.Value = true;
            
            // Shadow-Eigenschaft demonstrieren
            checkBox.Shadow = true; // Enable shadow effect
            workbook.Save("CheckBoxWithShadow.xlsx");
            
            checkBox.Shadow = false; // Disable shadow effect
            workbook.Save("CheckBoxWithoutShadow.xlsx");
        }
    }
}
```

### Siehe auch

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


