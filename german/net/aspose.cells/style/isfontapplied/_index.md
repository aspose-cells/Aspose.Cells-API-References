---
title: "Style.IsFontApplied"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob die Schriftformatierung angewendet werden soll"
type: docs
url: /de/net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

Gibt an, ob die Schriftformatierung angewendet werden soll.

```csharp
public bool IsFontApplied { get; set; }
```

### Hinweise

Nur für benannte Stile.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFontAppliedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf eine Zelle aus dem Arbeitsblatt zu
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            
            // Ermitteln Sie den Stil der Zelle
            Style style = cell.GetStyle();
            
            // Schriftarteinstellungen anwenden
            style.Font.Name = "Times New Roman";
            style.Font.Size = 14;
            style.Font.Color = Color.Blue;
            
            // Aktiviere die Schriftanwendung
            style.IsFontApplied = true;
            
            // Setze den modifizierten Stil zurück in die Zelle
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontAppliedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


