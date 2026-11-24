---
title: "Font.IsItalic"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schriftart-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob die Schriftart kursiv ist"
type: docs
url: /de/net/aspose.cells/font/isitalic/
---
## Font.IsItalic property

Ruft einen Wert ab oder legt ihn fest, der angibt, ob die Schrift kursiv ist.

```csharp
public bool IsItalic { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsItalicDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf den Standardstil zu
            Style style = workbook.DefaultStyle;
            
            // Setzen Sie Schriftarteigenschaften einschließlich IsItalic
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.Font.IsItalic = true;
            
            // Den Stil auf Zelle A1 anwenden
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Italic Text Example");
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontPropertyIsItalicDemo.xlsx");
            
            // Kursiv-Eigenschaft überprüfen
            Console.WriteLine("Font is italic: " + cell.GetStyle().Font.IsItalic);
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


