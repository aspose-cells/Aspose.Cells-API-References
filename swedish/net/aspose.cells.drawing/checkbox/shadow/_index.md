---
title: "CheckBox.Shadow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBox-egenskap. Anger om combobox har 3D-skuggning"
type: docs
url: /sv/net/aspose.cells.drawing/checkbox/shadow/
---
## CheckBox.Shadow property

Anger om comboboxen har 3D-skuggning.

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
    public class CheckBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en kryssruta i kalkylbladet och hämta dess index
            int checkBoxIndex = sheet.CheckBoxes.Add(1, 1, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
            
            // Konfigurera kryssrutegenskaper
            checkBox.Text = "Enable Feature";
            checkBox.Value = true;
            
            // Demonstrera Shadow-egenskapen
            checkBox.Shadow = true; // Enable shadow effect
            workbook.Save("CheckBoxWithShadow.xlsx");
            
            checkBox.Shadow = false; // Disable shadow effect
            workbook.Save("CheckBoxWithoutShadow.xlsx");
        }
    }
}
```

### Se även

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


