---
title: "PasteOptions.OnlyVisibleCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PasteOptions-egenskap. True betyder att endast synliga celler kopieras"
type: docs
url: /sv/net/aspose.cells/pasteoptions/onlyvisiblecells/
---
## PasteOptions.OnlyVisibleCells property

Sant betyder att endast synliga celler kopieras.

```csharp
public bool OnlyVisibleCells { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOnlyVisibleCellsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med två kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Hämta celler från det första kalkylbladet och fyll i data
            Cells sourceCells = workbook.Worksheets[0].Cells;
            sourceCells["A1"].PutValue("Hidden A1");
            sourceCells["B2"].PutValue("Visible B2");
            sourceCells["C3"].PutValue("Hidden C3");
            
            // Dölj några rader och kolumner
            sourceCells.HideRow(0);  // Hides row 1 (A1)
            sourceCells.HideColumn(2); // Hides column C (C3)

            // Skapa källområde för kopiering
            Aspose.Cells.Range sourceRange = sourceCells.CreateRange("A1:C3");
            
            // Hämta celler från det andra kalkylbladet för destinationen
            Cells destCells = workbook.Worksheets[1].Cells;
            Aspose.Cells.Range destRange = destCells.CreateRange("A1:C3");
            
            // Skapa klistra in-alternativ och sätt OnlyVisibleCells
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.OnlyVisibleCells = true;
            
            // Kopiera endast synliga celler
            destRange.Copy(sourceRange, pasteOptions);
            
            // Skriv ut resultat för att demonstrera funktionaliteten
            Console.WriteLine("B2 value (should be copied): " + destCells["B2"].StringValue);
            Console.WriteLine("A1 value (should be empty): " + destCells["A1"].StringValue);
            Console.WriteLine("C3 value (should be empty): " + destCells["C3"].StringValue);
        }
    }
}
```

### Se även

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


