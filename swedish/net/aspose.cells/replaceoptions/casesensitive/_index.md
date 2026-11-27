---
title: "ReplaceOptions.CaseSensitive"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReplaceOptions egenskap. Anger om den sökta strängen är skiftlägeskänslig"
type: docs
url: /sv/net/aspose.cells/replaceoptions/casesensitive/
---
## ReplaceOptions.CaseSensitive property

Indikerar om den sökta strängen är skiftlägeskänslig.

```csharp
public bool CaseSensitive { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Skapa ersättningsalternativ med CaseSensitive = false
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            
            // Ersätt alla skiftlägesvarianter av "apple" med "orange"
            workbook.Replace("apple", "orange", options);

            // Skriv ut resultat
            Console.WriteLine("After replacement (CaseSensitive = false):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Återställ data
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Ändra till CaseSensitive = true
            options.CaseSensitive = true;
            workbook.Replace("apple", "orange", options);

            // Skriv ut resultat
            Console.WriteLine("\nAfter replacement (CaseSensitive = true):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Se även

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


