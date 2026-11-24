---
title: "Style.IsBorderApplied"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob die Rahmenformatierung angewendet werden soll."
type: docs
url: /de/net/aspose.cells/style/isborderapplied/
---
## Style.IsBorderApplied property

Gibt an, ob die Rahmenformatierung angewendet werden soll.

```csharp
public bool IsBorderApplied { get; set; }
```

### Hinweise

Nur für benannte Stile.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsBorderAppliedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie einen benutzerdefinierten Stil.
            Style style = workbook.CreateStyle();
            
            // Wenden Sie Rahmen-Einstellungen auf den Stil an.
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Black;
            
            // Prüfen Sie, ob der Rahmen angewendet wurde.
            Console.WriteLine("IsBorderApplied before setting: " + style.IsBorderApplied);
            
            // Setzen Sie IsBorderApplied explizit auf true.
            style.IsBorderApplied = true;
            
            // Wende den Stil auf eine Zelle an
            worksheet.Cells["A1"].SetStyle(style);
            
            // Überprüfen Sie die Anwendung des Rahmens.
            Console.WriteLine("IsBorderApplied after setting: " + style.IsBorderApplied);
            
            // Speichere die Arbeitsmappe
            workbook.Save("IsBorderAppliedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


