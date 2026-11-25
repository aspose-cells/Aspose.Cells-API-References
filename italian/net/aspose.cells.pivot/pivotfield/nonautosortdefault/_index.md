---
title: "PivotField.NonAutoSortDefault"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se un'operazione di ordinamento che verrà applicata a questo campo pivot è un'operazione di autosort o un semplice ordinamento dei dati."
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

Indica se un'operazione di ordinamento che verrà applicata a questo campo pivot è un'operazione di autosort o un semplice ordinamento dei dati.

```csharp
[Obsolete("Use !PivotField.SortSetting.IsSimpleSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool NonAutoSortDefault { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà !PivotField.SortSetting.IsSimpleSort. Questo metodo sarà rimosso tra 12 mesi a partire da settembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNonAutoSortDefaultDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al primo foglio di lavoro e alla tabella pivot
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Accedi al primo campo di riga nella tabella pivot
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Imposta la proprietà NonAutoSortDefault su true
            pivotField.NonAutoSortDefault = true;
            
            // Restituisci il valore della proprietà
            Console.WriteLine("NonAutoSortDefault property value: " + pivotField.NonAutoSortDefault);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


