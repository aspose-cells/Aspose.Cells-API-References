---
title: "ListObject.TableStyleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Получает и задаёт имя стиля таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listobject/tablestylename/
---
## ListObject.TableStyleName property

Получает и задает имя стиля таблицы

```csharp
public string TableStyleName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создать объект/таблицу списка
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Установить и отобразить стиль таблицы
            table.TableStyleName = "TableStyleLight15";
            Console.WriteLine("Table style name: " + table.TableStyleName);

            // Сохраните книгу
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


