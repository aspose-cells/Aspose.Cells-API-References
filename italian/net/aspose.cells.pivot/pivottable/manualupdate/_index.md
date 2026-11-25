---
title: "PivotTable.ManualUpdate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se il report della PivotTable viene ricalcolato solo su richiesta dell'utente"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/manualupdate/
---
## PivotTable.ManualUpdate property

Indica se il report PivotTable viene ricalcolato solo su richiesta dell'utente.

```csharp
public bool ManualUpdate { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyManualUpdateDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e riempilo con dati di esempio
            Worksheet dataSheet = workbook.Worksheets["Sheet1"];
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["A4"].PutValue("A");
            dataSheet.Cells["B4"].PutValue(30);

            // Aggiungi una tabella pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int index = pivotSheet.PivotTables.Add("Sheet1!A1:B4", "A3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];

            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Abilita aggiornamento manuale
            pivotTable.ManualUpdate = true;
            
            // A questo punto, la tabella pivot non verrà aggiornata automaticamente
            Console.WriteLine("Pivot table before refresh (ManualUpdate=true):");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will be empty
            
            // Aggiorna manualmente la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            Console.WriteLine("Pivot table after manual refresh:");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will show "40" (sum of category A)
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableManualUpdateDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


