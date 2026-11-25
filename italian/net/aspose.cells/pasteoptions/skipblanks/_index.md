---
title: "PasteOptions.SkipBlanks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PasteOptions. Indica se salta le celle vuote"
type: docs
url: /it/net/aspose.cells/pasteoptions/skipblanks/
---
## PasteOptions.SkipBlanks property

Indica se saltare le celle vuote.

```csharp
public bool SkipBlanks { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertySkipBlanksDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di origine con dati di esempio
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Riempi l'intervallo di origine con alcuni valori e celle vuote
            sourceSheet.Cells["A1"].PutValue("Value 1");
            sourceSheet.Cells["A2"].PutValue(""); // Blank cell
            sourceSheet.Cells["A3"].PutValue("Value 3");
            sourceSheet.Cells["A4"].PutValue(""); // Blank cell
            
            // Crea la cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Riempi l'intervallo di destinazione con valori esistenti
            destSheet.Cells["A1"].PutValue("Existing 1");
            destSheet.Cells["A2"].PutValue("Existing 2");
            destSheet.Cells["A3"].PutValue("Existing 3");
            destSheet.Cells["A4"].PutValue("Existing 4");
            
            // Ottieni intervalli con nomi di tipo completamente qualificati
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A4");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A4");
            
            // Copia con SkipBlanks = true (predefinito)
            destRange.Copy(sourceRange, new PasteOptions { SkipBlanks = true });
            
            Console.WriteLine("Results with SkipBlanks=true:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {destSheet.Cells[i, 0].StringValue}");
            }
            
            // Reimposta i valori di destinazione
            destSheet.Cells["A1"].PutValue("Existing 1");
            destSheet.Cells["A2"].PutValue("Existing 2");
            destSheet.Cells["A3"].PutValue("Existing 3");
            destSheet.Cells["A4"].PutValue("Existing 4");
            
            // Copia con SkipBlanks = false
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

### Vedi anche

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


