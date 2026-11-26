---
title: "DataModelTableCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataModelTableCollection. Получает таблицу модели данных по позиции в коллекции"
type: docs
url: /ru/net/aspose.cells.datamodels/datamodeltablecollection/item/
---
## DataModelTableCollection indexer (1 of 2)

Получает таблицу модели данных по позиции в коллекции.

```csharp
public DataModelTable this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Позиция в коллекции. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте примерные данные для таблицы
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Создать таблицу
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "EmployeeTable";

            // Получить доступ к DataModelTableCollection
            DataModelTableCollection dataModelTables = workbook.DataModel.Tables;

            // Продемонстрировать чтение свойства Item (индексатор)
            Console.WriteLine("Number of tables: " + dataModelTables.Count);
            for (int i = 0; i < dataModelTables.Count; i++)
            {
                DataModelTable tableItem = dataModelTables[i]; // Using Item property
                Console.WriteLine($"Table {i}: {tableItem.Name}");
            }

            // Добавьте еще одну таблицу, чтобы продемонстрировать несколько элементов
            worksheet.Cells["D1"].PutValue("DeptID");
            worksheet.Cells["E1"].PutValue("Department");
            worksheet.Cells["D2"].PutValue(101);
            worksheet.Cells["E2"].PutValue("HR");
            int secondTableIndex = worksheet.ListObjects.Add(3, 0, 1, 1, true);
            worksheet.ListObjects[secondTableIndex].DisplayName = "DepartmentTable";

            // Показать обновленную коллекцию
            Console.WriteLine("\nAfter adding second table:");
            for (int i = 0; i < dataModelTables.Count; i++)
            {
                Console.WriteLine($"Table {i}: {dataModelTables[i].Name}");
            }

            // Сохраните книгу
            workbook.Save("DataModelTableCollectionItemIndexDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataModelTable](../../datamodeltable/)
* class [DataModelTableCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)

---

## DataModelTableCollection indexer (2 of 2)

Получает таблицу модели данных по имени.

```csharp
public DataModelTable this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя таблицы модели данных. |

### Примеры

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

### См. также

* class [DataModelTable](../../datamodeltable/)
* class [DataModelTableCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


