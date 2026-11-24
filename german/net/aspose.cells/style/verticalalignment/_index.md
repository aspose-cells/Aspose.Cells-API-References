---
title: "Style.VerticalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt den vertikalen Ausrichtungstyp des Textes in einer Zelle zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/style/verticalalignment/
---
## Style.VerticalAlignment property

Liest oder setzt den vertikalen Ausrichtungstyp des Textes in einer Zelle.

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zugriff auf Zelle A1
            Cell cell = worksheet.Cells["A1"];
            
            // Setzen Sie den Zellenwert
            cell.PutValue("Vertical Alignment Demo");
            
            // Greifen Sie auf den Stil der Zelle zu
            Style style = cell.GetStyle();
            
            // Setze die vertikale Ausrichtung auf Oben
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("VerticalAlignmentDemo.xlsx");
            
            Console.WriteLine("Vertical alignment set to Top for cell A1.");
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


