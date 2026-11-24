---
title: "PasteOptions.SkipBlanks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PasteOptions-Eigenschaft. Gibt an, ob leere Zellen übersprungen werden"
type: docs
url: /de/net/aspose.cells/pasteoptions/skipblanks/
---
## PasteOptions.SkipBlanks property

Gibt an, ob leere Zellen übersprungen werden.

```csharp
public bool SkipBlanks { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertySkipBlanksDemo
    {
        public static void Run()
        {
            // Erstelle ein Quell‑Arbeitsbuch mit Beispieldaten
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Quellbereich mit einigen Werten und leeren Zellen füllen
            sourceSheet.Cells["A1"].PutValue("Value 1");
            sourceSheet.Cells["A2"].PutValue(""); // Blank cell
            sourceSheet.Cells["A3"].PutValue("Value 3");
            sourceSheet.Cells["A4"].PutValue(""); // Blank cell
            
            // Erstelle Ziel‑Arbeitsbuch
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Zielbereich mit vorhandenen Werten füllen
            destSheet.Cells["A1"].PutValue("Existing 1");
            destSheet.Cells["A2"].PutValue("Existing 2");
            destSheet.Cells["A3"].PutValue("Existing 3");
            destSheet.Cells["A4"].PutValue("Existing 4");
            
            // Bereiche mit vollständig qualifizierten Typnamen abrufen
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A4");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A4");
            
            // Kopieren mit SkipBlanks = true (Standard)
            destRange.Copy(sourceRange, new PasteOptions { SkipBlanks = true });
            
            Console.WriteLine("Results with SkipBlanks=true:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {destSheet.Cells[i, 0].StringValue}");
            }
            
            // Zielwerte zurücksetzen
            destSheet.Cells["A1"].PutValue("Existing 1");
            destSheet.Cells["A2"].PutValue("Existing 2");
            destSheet.Cells["A3"].PutValue("Existing 3");
            destSheet.Cells["A4"].PutValue("Existing 4");
            
            // Kopieren mit SkipBlanks = false
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

### Siehe auch

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


