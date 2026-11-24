---
title: "PasteOptions.OnlyVisibleCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PasteOptions-Eigenschaft. True bedeutet, dass nur sichtbare Zellen kopiert werden"
type: docs
url: /de/net/aspose.cells/pasteoptions/onlyvisiblecells/
---
## PasteOptions.OnlyVisibleCells property

True bedeutet, dass nur sichtbare Zellen kopiert werden.

```csharp
public bool OnlyVisibleCells { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOnlyVisibleCellsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe mit zwei Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Hole Zellen aus dem ersten Arbeitsblatt und fülle Daten ein
            Cells sourceCells = workbook.Worksheets[0].Cells;
            sourceCells["A1"].PutValue("Hidden A1");
            sourceCells["B2"].PutValue("Visible B2");
            sourceCells["C3"].PutValue("Hidden C3");
            
            // Verstecke einige Zeilen und Spalten
            sourceCells.HideRow(0);  // Hides row 1 (A1)
            sourceCells.HideColumn(2); // Hides column C (C3)

            // Erstelle den Quellbereich zum Kopieren
            Aspose.Cells.Range sourceRange = sourceCells.CreateRange("A1:C3");
            
            // Hole Zellen aus dem zweiten Arbeitsblatt für das Ziel
            Cells destCells = workbook.Worksheets[1].Cells;
            Aspose.Cells.Range destRange = destCells.CreateRange("A1:C3");
            
            // Erstelle PasteOptions und setze OnlyVisibleCells
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.OnlyVisibleCells = true;
            
            // Kopiere nur sichtbare Zellen
            destRange.Copy(sourceRange, pasteOptions);
            
            // Gib die Ergebnisse aus, um die Funktionalität zu demonstrieren
            Console.WriteLine("B2 value (should be copied): " + destCells["B2"].StringValue);
            Console.WriteLine("A1 value (should be empty): " + destCells["A1"].StringValue);
            Console.WriteLine("C3 value (should be empty): " + destCells["C3"].StringValue);
        }
    }
}
```

### Siehe auch

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


