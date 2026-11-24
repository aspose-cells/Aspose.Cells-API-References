---
title: "GroupBox.Shadow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GroupBox-Eigenschaft. Gibt an, ob die GroupBox einen Schatten hat"
type: docs
url: /de/net/aspose.cells.drawing/groupbox/shadow/
---
## GroupBox.Shadow property

Gibt an, ob die GroupBox einen Schatten hat.

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
    public class GroupBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge eine GroupBox mit Schatten hinzu
            GroupBox groupBoxWithShadow = worksheet.Shapes.AddGroupBox(1, 0, 1, 0, 200, 150);
            groupBoxWithShadow.Shadow = true;
            groupBoxWithShadow.Text = "GroupBox with Shadow";
            
            // Füge eine GroupBox ohne Schatten hinzu
            GroupBox groupBoxWithoutShadow = worksheet.Shapes.AddGroupBox(1, 2, 1, 0, 200, 150);
            groupBoxWithoutShadow.Shadow = false;
            groupBoxWithoutShadow.Text = "GroupBox without Shadow";
            
            // Füge Radio-Buttons innerhalb der GroupBoxes hinzu, um die Gruppierung zu demonstrieren
            RadioButton radio1 = worksheet.Shapes.AddRadioButton(3, 0, 2, 0, 30, 100);
            radio1.Text = "Option 1";
            radio1.LinkedCell = "A1";
            
            RadioButton radio2 = worksheet.Shapes.AddRadioButton(6, 0, 2, 0, 30, 100);
            radio2.Text = "Option 2";
            radio2.LinkedCell = "A1";
            
            // Gruppiere die Formen
            Shape[] shapes = { groupBoxWithShadow, radio1, radio2 };
            worksheet.Shapes.Group(shapes);
            
            // Speichere die Arbeitsmappe
            workbook.Save("GroupBoxShadowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GroupBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


