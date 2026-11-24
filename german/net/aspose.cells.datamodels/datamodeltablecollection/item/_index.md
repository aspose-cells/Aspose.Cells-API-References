---
title: "DataModelTableCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelTableCollection‑Eigenschaft. Gibt die Datentabelle des Modells anhand der Position in der Sammlung zurück"
type: docs
url: /de/net/aspose.cells.datamodels/datamodeltablecollection/item/
---
## DataModelTableCollection indexer (1 of 2)

Gibt die Datentabelle des Modells anhand der Position in der Sammlung zurück.

```csharp
public DataModelTable this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Die Position der Sammlung. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für eine Tabelle erstellen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Eine Tabelle erstellen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "EmployeeTable";

            // Greife auf die DataModelTableCollection zu
            DataModelTableCollection dataModelTables = workbook.DataModel.Tables;

            // Demonstrieren Sie das Lesen der Item-Eigenschaft (Indexer)
            Console.WriteLine("Number of tables: " + dataModelTables.Count);
            for (int i = 0; i < dataModelTables.Count; i++)
            {
                DataModelTable tableItem = dataModelTables[i]; // Using Item property
                Console.WriteLine($"Table {i}: {tableItem.Name}");
            }

            // Fügen Sie eine weitere Tabelle hinzu, um mehrere Elemente zu demonstrieren
            worksheet.Cells["D1"].PutValue("DeptID");
            worksheet.Cells["E1"].PutValue("Department");
            worksheet.Cells["D2"].PutValue(101);
            worksheet.Cells["E2"].PutValue("HR");
            int secondTableIndex = worksheet.ListObjects.Add(3, 0, 1, 1, true);
            worksheet.ListObjects[secondTableIndex].DisplayName = "DepartmentTable";

            // Aktualisierte Sammlung anzeigen
            Console.WriteLine("\nAfter adding second table:");
            for (int i = 0; i < dataModelTables.Count; i++)
            {
                Console.WriteLine($"Table {i}: {dataModelTables[i].Name}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("DataModelTableCollectionItemIndexDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataModelTable](../../datamodeltable/)
* class [DataModelTableCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)

---

## DataModelTableCollection indexer (2 of 2)

Ruft die Datemodell-Tabelle anhand des Namens ab.

```csharp
public DataModelTable this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Name der Datemodell-Tabelle. |

### Beispiele

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

### Siehe auch

* class [DataModelTable](../../datamodeltable/)
* class [DataModelTableCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


