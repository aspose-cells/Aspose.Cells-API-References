---
title: "ListBox.Shadow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBox-egenskap. Anger om kombinationsrutan har 3D-skuggning"
type: docs
url: /sv/net/aspose.cells.drawing/listbox/shadow/
---
## ListBox.Shadow property

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
    public class ListBoxPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i listobjekt
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Skapa listbox och ställ in grundegenskaperna
            ListBox listBox = worksheet.Shapes.AddListBox(2, 1, 5, 1, 100, 150);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            // Ställ in skuggegenskapen
            listBox.Shadow = true;

            // Spara och ladda om för att verifiera
            workbook.Save("ListBoxShadowDemo.xlsx");
            
            Workbook loadedWorkbook = new Workbook("ListBoxShadowDemo.xlsx");
            ListBox loadedBox = (ListBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Shadow enabled: " + loadedBox.Shadow);
        }
    }
}
```

### Se även

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


