---
title: "ListObject.DisplayName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Возвращает и задает отображаемое имя таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listobject/displayname/
---
## ListObject.DisplayName property

Получает и задает отображаемое имя таблицы.

```csharp
public string DisplayName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);

            // Создать объект списка
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Установить отображаемое имя и продемонстрировать его использование
            listObject.DisplayName = "ProductTable";
            Console.WriteLine("List Object Display Name: " + listObject.DisplayName);

            // Сохраните книгу
            workbook.Save("ListObjectDisplayNameDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


