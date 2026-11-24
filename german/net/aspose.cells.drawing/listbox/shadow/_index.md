---
title: "ListBox.Shadow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBox-Eigenschaft. Gibt an, ob die ComboBox eine 3D-Schattierung hat"
type: docs
url: /de/net/aspose.cells.drawing/listbox/shadow/
---
## ListBox.Shadow property

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
    public class ListBoxPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Listenelemente befüllen
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Erstelle ListBox und setze Kern‑Eigenschaften
            ListBox listBox = worksheet.Shapes.AddListBox(2, 1, 5, 1, 100, 150);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            // Setze Schatten‑Eigenschaft
            listBox.Shadow = true;

            // Speichern und neu laden, um zu überprüfen
            workbook.Save("ListBoxShadowDemo.xlsx");
            
            Workbook loadedWorkbook = new Workbook("ListBoxShadowDemo.xlsx");
            ListBox loadedBox = (ListBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Shadow enabled: " + loadedBox.Shadow);
        }
    }
}
```

### Siehe auch

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


