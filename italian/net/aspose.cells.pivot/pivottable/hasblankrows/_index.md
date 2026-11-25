---
title: "PivotTable.HasBlankRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se aggiungere righe vuote. Questa proprietà si applica solo ai tipi di formato automatico della PivotTable che richiedono l'aggiunta di righe vuote"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/hasblankrows/
---
## PivotTable.HasBlankRows property

Indica se aggiungere righe vuote. Questa proprietà si applica solo ai tipi di formato automatico della PivotTable che richiedono l'aggiunta di righe vuote.

```csharp
[Obsolete("Use PivotField.InsertBlankRow property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBlankRows { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotField.InsertBlankRow. Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyHasBlankRowsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet dataSheet = wb.Worksheets[0];
            
            // Crea dati di esempio
            dataSheet.Cells[0, 0].PutValue("Category");
            dataSheet.Cells[0, 1].PutValue("Product");
            dataSheet.Cells[0, 2].PutValue("Sales");
            
            Random rnd = new Random();
            for (int i = 1; i <= 10; i++)
            {
                dataSheet.Cells[i, 0].PutValue(rnd.Next(2) == 0 ? "Electronics" : "Furniture");
                dataSheet.Cells[i, 1].PutValue("Product " + rnd.Next(1, 4));
                dataSheet.Cells[i, 2].PutValue(rnd.Next(100, 1000));
            }

            // Aggiungi tabella pivot
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Sheet1!A1:C11", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
            
            // Dimostra la proprietà HasBlankRows
            pivotTable.HasBlankRows = false; // Remove blank lines between items
            
            // Salva la cartella di lavoro
            wb.Save("PivotTableHasBlankRowsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


