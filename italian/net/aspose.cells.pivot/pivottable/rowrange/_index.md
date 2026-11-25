---
title: "PivotTable.RowRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area di riga nel report della PivotTable. Sola lettura"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/rowrange/
---
## PivotTable.RowRange property

Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'area di riga nel report della PivotTable. Sola lettura.

```csharp
public CellArea RowRange { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowRangeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Aggiorna tutte le tabelle pivot nella cartella di lavoro
            workbook.Worksheets.RefreshAll();
            
            // Ottieni la prima tabella pivot dal primo foglio di lavoro
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[0];
            
            // Ottieni l'intervallo di riga della tabella pivot
            CellArea rowRange = pivotTable.RowRange;
            
            // Visualizza le coordinate dell'intervallo di riga
            Console.WriteLine("PivotTable Row Range:");
            Console.WriteLine($"Start Row: {rowRange.StartRow}");
            Console.WriteLine($"End Row: {rowRange.EndRow}");
            Console.WriteLine($"Start Column: {rowRange.StartColumn}");
            Console.WriteLine($"End Column: {rowRange.EndColumn}");
            
            // Ottieni l'intervallo di colonna della tabella pivot
            CellArea columnRange = pivotTable.ColumnRange;
            
            // Visualizza le coordinate dell'intervallo di colonna
            Console.WriteLine("\nPivotTable Column Range:");
            Console.WriteLine($"Start Row: {columnRange.StartRow}");
            Console.WriteLine($"End Row: {columnRange.EndRow}");
            Console.WriteLine($"Start Column: {columnRange.StartColumn}");
            Console.WriteLine($"End Column: {columnRange.EndColumn}");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


