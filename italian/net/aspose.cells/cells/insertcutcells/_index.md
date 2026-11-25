---
title: "Cells.InsertCutCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Inserisci l'intervallo tagliato"
type: docs
url: /it/net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

Inserisci intervallo tagliato.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cutRange | Intervallo | L'intervallo tagliato. |
| riga | Int32 | La riga. |
| colonna | Int32 | La colonna. |
| shiftType | ShiftType | Indica come spostare gli altri oggetti dell'intervallo di destinazione quando si inserisce l'intervallo tagliato. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertCutCellsWithRangeInt32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e alle sue celle
            Worksheet sourceSheet = workbook.Worksheets[0];
            Cells sourceCells = sourceSheet.Cells;
            
            // Aggiungi alcuni dati alle celle di origine
            sourceCells["A1"].PutValue("Source A1");
            sourceCells["B1"].PutValue("Source B1");
            sourceCells["A2"].PutValue("Source A2");
            sourceCells["B2"].PutValue("Source B2");
            
            // Crea un secondo foglio di lavoro come destinazione
            Worksheet destSheet = workbook.Worksheets.Add("Sheet2");
            Cells destCells = destSheet.Cells;
            
            // Aggiungi alcuni dati iniziali alla destinazione
            destCells["A1"].PutValue("Dest A1");
            destCells["B1"].PutValue("Dest B1");
            
            // Crea un intervallo da tagliare (A1:B2 dal foglio di origine)
            Aspose.Cells.Range cutRange = sourceCells.CreateRange("A1:B2");
            
            // Inserisci le celle tagliate in B2 nel foglio di destinazione, spostando le celle verso il basso
            destCells.InsertCutCells(cutRange, 1, 1, ShiftType.Down);
            
            // Salva la cartella di lavoro
            workbook.Save("InsertCutCellsDemo.xlsx");
            
            Console.WriteLine("InsertCutCells demo executed successfully.");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


