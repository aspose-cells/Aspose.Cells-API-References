---
title: "Klass DataModelTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataModels.DataModelTable klass. Representerar egenskaperna för en enskild tabell i kalkylbladets datamodell"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodeltable/
---
## DataModelTable class

Representerar egenskaper för en enskild tabell i kalkylbladets datamodell.

```csharp
public class DataModelTable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ConnectionName](../../aspose.cells.datamodels/datamodeltable/connectionname/) { get; } | Hämtar anslutningsnamnet för datamodelltabellen. |
| [Id](../../aspose.cells.datamodels/datamodeltable/id/) { get; } | Hämtar id för datamodelltabellen. |
| [Name](../../aspose.cells.datamodels/datamodeltable/name/) { get; } | Hämtar namnet på datamodelltabellen. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa en tabell
            worksheet.Cells["A1"].PutValue("ProductID");
            worksheet.Cells["B1"].PutValue("ProductName");
            worksheet.Cells["A2"].PutValue(101);
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["A3"].PutValue(102);
            worksheet.Cells["B3"].PutValue("Monitor");

            // Skapa ett ListObject (tabell)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "ProductsTable";

            // Få åtkomst till DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Visa DataModelTable-egenskaper
            Console.WriteLine("Data Model Table Properties:");
            Console.WriteLine($"ID: {dataModelTable.Id}");
            Console.WriteLine($"Name: {dataModelTable.Name}");
            Console.WriteLine($"Connection Name: {dataModelTable.ConnectionName}");

            // Skapa en pivottabell med hjälp av DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ProductName");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "ProductID");

            // Spara arbetsboken
            workbook.Save("DataModelTableDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


