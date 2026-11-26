---
title: "DataModelTable.ConnectionName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataModelTable. Возвращает имя соединения таблицы модели данных"
type: docs
url: /ru/net/aspose.cells.datamodels/datamodeltable/connectionname/
---
## DataModelTable.ConnectionName property

Получает имя соединения таблицы модели данных.

```csharp
public string ConnectionName { get; }
```

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для создания таблицы
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("John Doe");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Jane Smith");

            // Создать ListObject (таблица)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "OrdersTable";

            // Получить доступ к DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Отобразить текущее значение ConnectionName
            Console.WriteLine("Current ConnectionName: " + dataModelTable.ConnectionName);

            // Создать сводную таблицу, используя соединение DataModelTable
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Customer");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "OrderID");

            // Примечание: ConnectionName только для чтения, поэтому мы не можем установить его
            // Это демонстрирует, как использовать существующее имя соединения
            if (!string.IsNullOrEmpty(dataModelTable.ConnectionName))
            {
                Console.WriteLine("This table is connected via: " + dataModelTable.ConnectionName);
            }

            // Сохраните книгу
            workbook.Save("DataModelTableConnectionNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


