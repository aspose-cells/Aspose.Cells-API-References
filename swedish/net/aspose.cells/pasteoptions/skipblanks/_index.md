---
title: "PasteOptions.SkipBlanks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PasteOptions-egenskap. Anger om tomma celler ska hoppas över"
type: docs
url: /sv/net/aspose.cells/pasteoptions/skipblanks/
---
## PasteOptions.SkipBlanks property

Anger om tomma celler ska hoppas över.

```csharp
public bool SkipBlanks { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertySkipBlanksDemo
    {
        public static void Run()
        {
            // Skapa en källarbetsbok med exempeldata
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Fyll källområdet med några värden och tomma celler
            sourceSheet.Cells["A1"].PutValue("Value 1");
            sourceSheet.Cells["A2"].PutValue(""); // Blank cell
            sourceSheet.Cells["A3"].PutValue("Value 3");
            sourceSheet.Cells["A4"].PutValue(""); // Blank cell
            
            // Skapa målarbetsbok
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Fyll destinationsområdet med befintliga värden
            destSheet.Cells["A1"].PutValue("Existing 1");
            destSheet.Cells["A2"].PutValue("Existing 2");
            destSheet.Cells["A3"].PutValue("Existing 3");
            destSheet.Cells["A4"].PutValue("Existing 4");
            
            // Hämta områden med fullständigt kvalificerade typnamn
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A4");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A4");
            
            // Kopiera med SkipBlanks = true (standard)
            destRange.Copy(sourceRange, new PasteOptions { SkipBlanks = true });
            
            Console.WriteLine("Results with SkipBlanks=true:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {destSheet.Cells[i, 0].StringValue}");
            }
            
            // Återställ destinationsvärden
            destSheet.Cells["A1"].PutValue("Existing 1");
            destSheet.Cells["A2"].PutValue("Existing 2");
            destSheet.Cells["A3"].PutValue("Existing 3");
            destSheet.Cells["A4"].PutValue("Existing 4");
            
            // Kopiera med SkipBlanks = false
            destRange.Copy(sourceRange, new PasteOptions { SkipBlanks = false });
            
            Console.WriteLine("\nResults with SkipBlanks=false:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {destSheet.Cells[i, 0].StringValue}");
            }
        }
    }
}
```

### Se även

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


