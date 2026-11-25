---
title: "PivotFilter.FilterType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotFilter property. Ottiene il tipo di filtro del filtro pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/filtertype/
---
## PivotFilter.FilterType property

Ottiene il tipo di filtro del filtro pivot.

```csharp
public PivotFilterType FilterType { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al primo foglio di lavoro e alla tabella pivot
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Applica un filtro di valore (minore di 2) al primo campo base
            pivotTable.BaseFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 2, 0);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Ricarica la cartella di lavoro per verificare il filtro
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            PivotTable verifyPivotTable = verifyWorkbook.Worksheets[0].PivotTables[0];
            
            // Ottieni il filtro applicato e dimostra la proprietà FilterType
            PivotFilter filter = verifyPivotTable.BaseFields[0].GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType); // Should output ValueLessThan
            Console.WriteLine("Filter Value: " + filter.GetNumberValues()[0]); // Should output 2
        }
    }
}
```

### Vedi anche

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


