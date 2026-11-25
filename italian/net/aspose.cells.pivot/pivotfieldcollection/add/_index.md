---
title: "PivotFieldCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFieldCollection. Aggiunge un oggetto PivotField al tipo specifico PivotFields"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldcollection/add/
---
## PivotFieldCollection.Add method

Aggiunge un oggetto PivotField al tipo specifico PivotFields.

```csharp
public int Add(PivotField pivotField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotField | PivotField | Un oggetto PivotField. |

### Valore di ritorno

L'indice dell'oggetto PivotField in questi PivotFields.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddWithPivotFieldDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("sample_pivot_table.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Aggiorna i dati della tabella pivot
            pivotTable.RefreshData();
            
            // Aggiungi campo dati all'area dei campi colonna usando il metodo Add
            pivotTable.ColumnFields.Add(pivotTable.DataField);
            
            // Calcola i dati della tabella pivot
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("output_pivot_table.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


