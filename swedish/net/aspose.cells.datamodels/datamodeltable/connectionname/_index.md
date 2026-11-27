---
title: "Skapa en pivottabell med DataModelTable:s anslutning"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Obs: ConnectionName är skrivskyddad, så vi kan inte sätta den"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodeltable/connectionname/
---
## DataModelTable.ConnectionName property

Hämtar anslutningsnamnet för datamodelltabellen.

```csharp
public string ConnectionName { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa en tabell
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("John Doe");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Jane Smith");

            // Skapa ett ListObject (tabell)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "OrdersTable";

            // Få åtkomst till DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Detta demonstrerar hur man använder det befintliga anslutningsnamnet
            Console.WriteLine("Current ConnectionName: " + dataModelTable.ConnectionName);

            // Skapa en pivottabell med hjälp av DataModelTable:s anslutning
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Customer");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "OrderID");

            // Obs: ConnectionName är skrivskyddad, så vi kan inte ändra den
            // Detta demonstrerar hur man använder det befintliga anslutningsnamnet
            if (!string.IsNullOrEmpty(dataModelTable.ConnectionName))
            {
                Console.WriteLine("This table is connected via: " + dataModelTable.ConnectionName);
            }

            // Spara arbetsboken
            workbook.Save("DataModelTableConnectionNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


