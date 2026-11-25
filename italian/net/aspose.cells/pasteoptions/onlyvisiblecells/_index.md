---
title: "PasteOptions.OnlyVisibleCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PasteOptions. True significa copiare solo le celle visibili"
type: docs
url: /it/net/aspose.cells/pasteoptions/onlyvisiblecells/
---
## PasteOptions.OnlyVisibleCells property

True indica che vengono copiate solo le celle visibili.

```csharp
public bool OnlyVisibleCells { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOnlyVisibleCellsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con due fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Ottieni le celle dal primo foglio di lavoro e popola i dati
            Cells sourceCells = workbook.Worksheets[0].Cells;
            sourceCells["A1"].PutValue("Hidden A1");
            sourceCells["B2"].PutValue("Visible B2");
            sourceCells["C3"].PutValue("Hidden C3");
            
            // Nascondi alcune righe e colonne
            sourceCells.HideRow(0);  // Hides row 1 (A1)
            sourceCells.HideColumn(2); // Hides column C (C3)

            // Crea l'intervallo di origine da copiare
            Aspose.Cells.Range sourceRange = sourceCells.CreateRange("A1:C3");
            
            // Ottieni le celle dal secondo foglio di lavoro per la destinazione
            Cells destCells = workbook.Worksheets[1].Cells;
            Aspose.Cells.Range destRange = destCells.CreateRange("A1:C3");
            
            // Crea le opzioni di incolla e imposta OnlyVisibleCells
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.OnlyVisibleCells = true;
            
            // Copia solo le celle visibili
            destRange.Copy(sourceRange, pasteOptions);
            
            // Genera i risultati per dimostrare la funzionalità
            Console.WriteLine("B2 value (should be copied): " + destCells["B2"].StringValue);
            Console.WriteLine("A1 value (should be empty): " + destCells["A1"].StringValue);
            Console.WriteLine("C3 value (should be empty): " + destCells["C3"].StringValue);
        }
    }
}
```

### Vedi anche

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


