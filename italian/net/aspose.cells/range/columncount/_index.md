---
title: "Range.ColumnCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Restituisce il numero di colonne nell'intervallo"
type: docs
url: /it/net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

Ottiene il conteggio delle colonne nell'intervallo.

```csharp
public int ColumnCount { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crea dati di esempio (5 colonne x 3 righe)
            for (int col = 0; col < 5; col++)
            {
                for (int row = 0; row < 3; row++)
                {
                    sheet.Cells[row, col].PutValue($"Data {row},{col}");
                }
            }
            
            // Crea un intervallo che copre tutte le colonne dei dati
            Aspose.Cells.Range dataRange = sheet.Cells.CreateRange(0, 0, 3, 5);
            
            // Dimostra l'uso di ColumnCount
            Console.WriteLine($"Range has {dataRange.ColumnCount} columns");
            
            // Adatta automaticamente ogni colonna nell'intervallo
            for (int i = 0; i < dataRange.ColumnCount; i++)
            {
                sheet.AutoFitColumn(dataRange.FirstColumn + i);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


