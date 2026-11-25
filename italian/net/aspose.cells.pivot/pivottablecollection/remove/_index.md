---
title: "PivotTableCollection.Remove"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTableCollection. Elimina la PivotTable specificata e rimuove i dati della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottablecollection/remove/
---
## Remove(PivotTable) {#remove}

Elimina il PivotTable specificato e elimina i dati del PivotTable

```csharp
public void Remove(PivotTable pivotTable)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | PivotTable | Oggetto PivotTable |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ottieni la collezione di tabelle pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            
            // Verifica se ci sono tabelle pivot
            if (pivotTables.Count > 0)
            {
                // Ottieni la prima tabella pivot
                PivotTable pivotTable = pivotTables[0];
                
                // Rimuovi la tabella pivot
                pivotTables.Remove(pivotTable);
                
                Console.WriteLine("Pivot table removed successfully. Count: " + pivotTables.Count);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableRemoved.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Remove(PivotTable, bool) {#remove_1}

Elimina il PivotTable specificato

```csharp
public void Remove(PivotTable pivotTable, bool keepData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | PivotTable | Oggetto PivotTable |
| keepData | Booleano | Indica se mantenere i dati della PivotTable |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Aggiungi una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "D5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Dimostra il metodo Remove con PivotTable e parametri booleani
            Console.WriteLine("Before removal - Cell D5 value: " + worksheet.Cells["D5"].StringValue);
            
            // Rimuovi la tabella pivot ma conserva i dati (true)
            worksheet.PivotTables.Remove(pivotTable, true);
            Console.WriteLine("After removal (keep data) - Cell D5 value: " + worksheet.Cells["D5"].StringValue);

            // Aggiungi un'altra tabella pivot
            index = worksheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nBefore removal - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
            
            // Rimuovi la tabella pivot e cancella i dati (false)
            worksheet.PivotTables.Remove(pivotTable, false);
            Console.WriteLine("After removal (clear data) - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


