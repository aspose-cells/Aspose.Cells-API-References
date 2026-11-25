---
title: "Classe DataModelTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DataModels.DataModelTable. Rappresenta le proprietà di una singola tabella nel modello di dati del foglio di calcolo"
type: docs
url: /it/net/aspose.cells.datamodels/datamodeltable/
---
## DataModelTable class

Rappresenta le proprietà di una singola tabella nel modello di dati del foglio di calcolo.

```csharp
public class DataModelTable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ConnectionName](../../aspose.cells.datamodels/datamodeltable/connectionname/) { get; } | Ottiene il nome della connessione della tabella del modello di dati. |
| [Id](../../aspose.cells.datamodels/datamodeltable/id/) { get; } | Ottiene l'ID della tabella del modello di dati. |
| [Name](../../aspose.cells.datamodels/datamodeltable/name/) { get; } | Ottiene il nome della tabella del modello di dati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelsClassDataModelTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare una tabella
            worksheet.Cells["A1"].PutValue("ProductID");
            worksheet.Cells["B1"].PutValue("ProductName");
            worksheet.Cells["A2"].PutValue(101);
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["A3"].PutValue(102);
            worksheet.Cells["B3"].PutValue("Monitor");

            // Crea un ListObject (tabella)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "ProductsTable";

            // Accedi al DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Visualizza le proprietà del DataModelTable
            Console.WriteLine("Data Model Table Properties:");
            Console.WriteLine($"ID: {dataModelTable.Id}");
            Console.WriteLine($"Name: {dataModelTable.Name}");
            Console.WriteLine($"Connection Name: {dataModelTable.ConnectionName}");

            // Crea una tabella pivot utilizzando il DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ProductName");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "ProductID");

            // Salva la cartella di lavoro
            workbook.Save("DataModelTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


