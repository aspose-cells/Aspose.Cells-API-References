---
title: "PivotTable.GetHorizontalPageBreaks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Ottiene le interruzioni di pagina orizzontali di questa tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/gethorizontalpagebreaks/
---
## PivotTable.GetHorizontalPageBreaks method

Ottiene le interruzioni di pagina orizzontali di questa tabella pivot.

```csharp
public int[] GetHorizontalPageBreaks()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file sorgente
            Workbook workbook = new Workbook("pivot_pagebreaks.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Aggiorna e calcola i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Ottieni interruzioni di pagina orizzontali
            int[] pageBreaks = pivotTable.GetHorizontalPageBreaks();
            
            // Visualizza i risultati
            Console.WriteLine("Horizontal Page Breaks:");
            foreach (int row in pageBreaks)
            {
                Console.WriteLine("Row: " + row);
            }
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


