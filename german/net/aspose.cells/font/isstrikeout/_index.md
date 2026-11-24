---
title: "Font.IsStrikeout"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schriftart-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob die Schriftart einfach durchgestrichen ist"
type: docs
url: /de/net/aspose.cells/font/isstrikeout/
---
## Font.IsStrikeout property

Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Schrift einfach durchgestrichen ist.

```csharp
public bool IsStrikeout { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsStrikeoutDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Methode 1: Durchstreichung direkt über den Stil festlegen
            Cell cell1 = worksheet.Cells["A1"];
            Style style1 = cell1.GetStyle();
            style1.Font.IsStrikeout = true;
            cell1.SetStyle(style1);
            cell1.PutValue("Strikeout Text (Style)");
            
            // Methode 2: Durchstreichung über HTML festlegen
            Cell cell2 = worksheet.Cells["A2"];
            cell2.HtmlString = "<s>Strikeout Text (HTML)</s>";
            
            // Durchstreichungs-Eigenschaft überprüfen
            Console.WriteLine("A1 IsStrikeout: " + cell1.GetStyle().Font.IsStrikeout);
            Console.WriteLine("A2 IsStrikeout: " + cell2.GetStyle().Font.IsStrikeout);
            
            // Zur Überprüfung speichern
            workbook.Save("FontStrikeoutDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


