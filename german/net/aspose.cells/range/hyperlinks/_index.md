---
title: "Range.Hyperlinks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt alle Hyperlinks im Bereich zurück"
type: docs
url: /de/net/aspose.cells/range/hyperlinks/
---
## Range.Hyperlinks property

Liefert alle Hyperlinks im Bereich.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einen Hyperlink zu Zelle A1 hinzu
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Erstelle einen Bereich, der A1 enthält
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1");
            
            // Erhalte Hyperlinks im Bereich
            Hyperlink[] hyperlinks = range.Hyperlinks;
            
            // Zeige Hyperlink-Informationen an
            if (hyperlinks.Length > 0)
            {
                Console.WriteLine("Hyperlink found:");
                Console.WriteLine($"Address: {hyperlinks[0].Address}");
                Console.WriteLine($"Link Type: {hyperlinks[0].LinkType}");
                
                // Den Hyperlink löschen
                hyperlinks[0].Delete();
                Console.WriteLine("Hyperlink deleted");
            }
            
            // Überprüfen, ob der Hyperlink entfernt wurde
            Console.WriteLine($"Total hyperlinks in worksheet: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### Siehe auch

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


