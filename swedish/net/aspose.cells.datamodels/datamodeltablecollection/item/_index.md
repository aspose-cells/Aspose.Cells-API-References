---
title: "DataModelTableCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataModelTableCollection egenskap. Hämtar datamodelltabellen efter position i samlingen"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodeltablecollection/item/
---
## DataModelTableCollection indexer (1 of 2)

Hämtar datamodelltabellen efter position i samlingen.

```csharp
public DataModelTable this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Positionen i samlingen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTableCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för en tabell
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Skapa en tabell
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "EmployeeTable";

            // Kom åt DataModelTableCollection
            DataModelTableCollection dataModelTables = workbook.DataModel.Tables;

            // Demonstrera läsning av Item-egenskapen (indexerare)
            Console.WriteLine("Number of tables: " + dataModelTables.Count);
            for (int i = 0; i < dataModelTables.Count; i++)
            {
                DataModelTable tableItem = dataModelTables[i]; // Using Item property
                Console.WriteLine($"Table {i}: {tableItem.Name}");
            }

            // Lägg till en annan tabell för att demonstrera flera objekt.
            worksheet.Cells["D1"].PutValue("DeptID");
            worksheet.Cells["E1"].PutValue("Department");
            worksheet.Cells["D2"].PutValue(101);
            worksheet.Cells["E2"].PutValue("HR");
            int secondTableIndex = worksheet.ListObjects.Add(3, 0, 1, 1, true);
            worksheet.ListObjects[secondTableIndex].DisplayName = "DepartmentTable";

            // Visa uppdaterad samling
            Console.WriteLine("\nAfter adding second table:");
            for (int i = 0; i < dataModelTables.Count; i++)
            {
                Console.WriteLine($"Table {i}: {dataModelTables[i].Name}");
            }

            // Spara arbetsboken
            workbook.Save("DataModelTableCollectionItemIndexDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataModelTable](../../datamodeltable/)
* class [DataModelTableCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)

---

## DataModelTableCollection indexer (2 of 2)

Hämtar datamodelltabellen efter namn.

```csharp
public DataModelTable this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Namnet på datamodelltabellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Widget");
            worksheet.Cells["B2"].PutValue(49.99);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "InventoryTable";

            DataModelTableCollection dataModelTables = workbook.DataModel.Tables;
            DataModelTable dataModelTable = dataModelTables["InventoryTable"];

            Console.WriteLine("Initial Table Name: " + dataModelTable.Name);

            worksheet.ListObjects[0].DisplayName = "UpdatedInventory";
            dataModelTable = dataModelTables["UpdatedInventory"];
            Console.WriteLine("Updated Table Name: " + dataModelTable.Name);

            workbook.Save("DataModelTableCollectionItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataModelTable](../../datamodeltable/)
* class [DataModelTableCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


