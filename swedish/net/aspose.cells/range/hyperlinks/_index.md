---
title: "Range.Hyperlinks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑egenskap. Hämtar alla hyperlänkar i området"
type: docs
url: /sv/net/aspose.cells/range/hyperlinks/
---
## Range.Hyperlinks property

Hämtar alla hyperlänkar i området.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Exempel

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
            
            // Lägg till en hyperlänk till cell A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Skapa ett område som innehåller A1
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1");
            
            // Hämta hyperlänkar i området
            Hyperlink[] hyperlinks = range.Hyperlinks;
            
            // Visa hyperlänkinformation
            if (hyperlinks.Length > 0)
            {
                Console.WriteLine("Hyperlink found:");
                Console.WriteLine($"Address: {hyperlinks[0].Address}");
                Console.WriteLine($"Link Type: {hyperlinks[0].LinkType}");
                
                // Ta bort hyperlänken
                hyperlinks[0].Delete();
                Console.WriteLine("Hyperlink deleted");
            }
            
            // Verifiera att hyperlänken har tagits bort
            Console.WriteLine($"Total hyperlinks in worksheet: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### Se även

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


