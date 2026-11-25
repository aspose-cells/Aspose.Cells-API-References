---
title: "DataModelTable.ConnectionName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataModelTable. Ottiene il nome della connessione della tabella del modello di dati"
type: docs
url: /it/net/aspose.cells.datamodels/datamodeltable/connectionname/
---
## DataModelTable.ConnectionName property

Ottiene il nome della connessione della tabella del modello di dati.

```csharp
public string ConnectionName { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelTablePropertyConnectionNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare una tabella
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("John Doe");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Jane Smith");

            // Crea un ListObject (tabella)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "OrdersTable";

            // Accedi al DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Visualizza il valore corrente di ConnectionName
            Console.WriteLine("Current ConnectionName: " + dataModelTable.ConnectionName);

            // Crea una tabella pivot utilizzando la connessione di DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Customer");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "OrderID");

            // Nota: ConnectionName è di sola lettura, quindi non possiamo impostarla
            // Questo dimostra come utilizzare il nome della connessione esistente
            if (!string.IsNullOrEmpty(dataModelTable.ConnectionName))
            {
                Console.WriteLine("This table is connected via: " + dataModelTable.ConnectionName);
            }

            // Salva la cartella di lavoro
            workbook.Save("DataModelTableConnectionNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


