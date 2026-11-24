---
title: "Cell.IsRichText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt an, ob der Zeichenkettenwert dieser Zelle ein reich formatierter Text ist"
type: docs
url: /de/net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

Gibt an, ob der Zeichenkettenwert dieser Zelle ein reich formatierter Text ist.

```csharp
public bool IsRichText()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodIsRichTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Eine Zelle mit Rich-Text-Formatierung erstellen
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello World");
            
            // Rich-Text-Formatierung anwenden
            FontSetting boldFont = cell.GetCharacters()[0];
            boldFont.Font.IsBold = true;
            
            FontSetting normalFont = cell.GetCharacters()[6];
            normalFont.Font.IsBold = false;
            
            // Prüfen, ob die Zelle Rich Text enthält
            bool isRichText = cell.IsRichText();
            Console.WriteLine("Is cell A1 rich text? " + isRichText);
            
            // Speichere die Arbeitsmappe
            workbook.Save("RichTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


