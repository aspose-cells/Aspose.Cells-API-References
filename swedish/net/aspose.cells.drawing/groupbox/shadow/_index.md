---
title: "GroupBox.Shadow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GroupBox-egenskap. Anger om groupboxen har skugga"
type: docs
url: /sv/net/aspose.cells.drawing/groupbox/shadow/
---
## GroupBox.Shadow property

Anger om grupprutan har skugga.

```csharp
public bool Shadow { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en gruppruta med skugga
            GroupBox groupBoxWithShadow = worksheet.Shapes.AddGroupBox(1, 0, 1, 0, 200, 150);
            groupBoxWithShadow.Shadow = true;
            groupBoxWithShadow.Text = "GroupBox with Shadow";
            
            // Lägg till en gruppruta utan skugga
            GroupBox groupBoxWithoutShadow = worksheet.Shapes.AddGroupBox(1, 2, 1, 0, 200, 150);
            groupBoxWithoutShadow.Shadow = false;
            groupBoxWithoutShadow.Text = "GroupBox without Shadow";
            
            // Lägg till radioknappar i grupprutorna för att demonstrera gruppering
            RadioButton radio1 = worksheet.Shapes.AddRadioButton(3, 0, 2, 0, 30, 100);
            radio1.Text = "Option 1";
            radio1.LinkedCell = "A1";
            
            RadioButton radio2 = worksheet.Shapes.AddRadioButton(6, 0, 2, 0, 30, 100);
            radio2.Text = "Option 2";
            radio2.LinkedCell = "A1";
            
            // Gruppera formerna
            Shape[] shapes = { groupBoxWithShadow, radio1, radio2 };
            worksheet.Shapes.Group(shapes);
            
            // Spara arbetsboken
            workbook.Save("GroupBoxShadowDemo.xlsx");
        }
    }
}
```

### Se även

* class [GroupBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


