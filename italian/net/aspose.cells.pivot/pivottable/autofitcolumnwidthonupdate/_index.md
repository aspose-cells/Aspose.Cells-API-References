---
title: "PivotTable.AutofitColumnWidthOnUpdate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se adattare automaticamente la larghezza della colonna durante l'aggiornamento"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/
---
## PivotTable.AutofitColumnWidthOnUpdate property

Indica se adattare automaticamente la larghezza della colonna all'aggiornamento

```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutofitColumnWidthOnUpdateDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al foglio di lavoro contenente la tabella pivot
            Worksheet worksheet = workbook.Worksheets["PIVOT"];
            
            // Accedi alla tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Disabilita l'adattamento automatico della larghezza della colonna durante l'aggiornamento
            pivotTable.AutofitColumnWidthOnUpdate = false;
            
            // Aggiorna la tabella pivot per applicare le modifiche
            worksheet.RefreshPivotTables();
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            Console.WriteLine("PivotTable AutofitColumnWidthOnUpdate property set successfully.");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


