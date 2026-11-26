---
title: "Класс DataModelTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DataModels.DataModelTable. Представляет свойства единственной таблицы в модели данных электронной таблицы"
type: docs
url: /ru/net/aspose.cells.datamodels/datamodeltable/
---
## DataModelTable class

Представляет свойства отдельной таблицы в модели данных электронной таблицы.

```csharp
public class DataModelTable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ConnectionName](../../aspose.cells.datamodels/datamodeltable/connectionname/) { get; } | Получает имя соединения таблицы модели данных. |
| [Id](../../aspose.cells.datamodels/datamodeltable/id/) { get; } | Получает идентификатор таблицы модели данных. |
| [Name](../../aspose.cells.datamodels/datamodeltable/name/) { get; } | Получает имя таблицы модели данных. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для создания таблицы
            worksheet.Cells["A1"].PutValue("ProductID");
            worksheet.Cells["B1"].PutValue("ProductName");
            worksheet.Cells["A2"].PutValue(101);
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["A3"].PutValue(102);
            worksheet.Cells["B3"].PutValue("Monitor");

            // Создать ListObject (таблица)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "ProductsTable";

            // Получить доступ к DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Отобразить свойства DataModelTable
            Console.WriteLine("Data Model Table Properties:");
            Console.WriteLine($"ID: {dataModelTable.Id}");
            Console.WriteLine($"Name: {dataModelTable.Name}");
            Console.WriteLine($"Connection Name: {dataModelTable.ConnectionName}");

            // Создать сводную таблицу с использованием DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ProductName");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "ProductID");

            // Сохраните книгу
            workbook.Save("DataModelTableDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


