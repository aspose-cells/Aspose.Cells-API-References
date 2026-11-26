---
title: "DataModelTable.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataModelTable. Возвращает идентификатор таблицы модели данных"
type: docs
url: /ru/net/aspose.cells.datamodels/datamodeltable/id/
---
## DataModelTable.Id property

Получает идентификатор таблицы модели данных.

```csharp
public string Id { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTablePropertyIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для создания таблицы
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Item 2");

            // Создать ListObject (таблица)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Получить DataModelTable (это только для чтения в рабочей книге)
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Отобразить текущее значение Id
            Console.WriteLine("Current DataModelTable Id: " + dataModelTable.Id);

            // Примечание: Свойство Id только для чтения, поэтому мы не можем установить его
            // Это демонстрирует, как получить доступ к существующему Id и использовать его

            // Пример использования: сравнивайте ID таблиц при работе с несколькими таблицами
            DataModelTable secondTable = null;
            if (workbook.DataModel.Tables.Count > 1)
            {
                secondTable = workbook.DataModel.Tables[1];
                if (dataModelTable.Id != secondTable.Id)
                {
                    Console.WriteLine("Different table IDs detected");
                }
            }

            // Сохраните книгу
            workbook.Save("DataModelTableIdDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


