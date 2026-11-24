---
title: "CopyOptions.ExtendToAdjacentRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CopyOptions property. Gibt an, ob Bereiche beim Kopieren des Bereichs in einen angrenzenden Bereich erweitert werden sollen"
type: docs
url: /de/net/aspose.cells/copyoptions/extendtoadjacentrange/
---
## CopyOptions.ExtendToAdjacentRange property

Gibt an, ob Bereiche erweitert werden, wenn der Bereich in einen angrenzenden Bereich kopiert wird.

```csharp
public bool ExtendToAdjacentRange { get; set; }
```

### Hinweise

Wenn sie true ist, wird nur der Bereich des Hyperlinks erweitert, ohne einen neuen Hyperlink hinzuzufügen, wenn Hyperlinks in angrenzende Zeilen kopiert werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyExtendToAdjacentRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Füge einen Hyperlink zu Zelle A1 hinzu
            ws.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Erstelle Kopieroptionen und setze ExtendToAdjacentRange auf true
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ExtendToAdjacentRange = true;

            // Kopiere Zeile 0 nach Zeile 1 mit den Kopieroptionen
            ws.Cells.CopyRows(ws.Cells, 0, 1, 1, copyOptions);

            // Überprüfe, ob der Hyperlink auf den angrenzenden Bereich erweitert wurde
            Console.WriteLine("Hyperlink count after copy: " + ws.Hyperlinks.Count);
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


