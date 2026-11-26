---
title: "FindOptions.SearchOrderByRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Указывает, осуществляется ли порядок поиска по строкам или столбцам"
type: docs
url: /ru/net/aspose.cells/findoptions/searchorderbyrows/
---
## FindOptions.SearchOrderByRows property

Указывает, осуществляется ли порядок поиска по строкам или столбцам.

```csharp
public bool SearchOrderByRows { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchOrderByRowsDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и добавьте примерные данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните ячейки тестовыми данными (поиск "abc" в порядке столбцов)
            worksheet.Cells["A1"].PutValue("xyz");
            worksheet.Cells["B1"].PutValue("def");
            worksheet.Cells["A2"].PutValue("123");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("abc");
            worksheet.Cells["B3"].PutValue("789");

            // Создайте параметры поиска и установите порядок поиска по столбцам
            FindOptions findOptions = new FindOptions();
            findOptions.SearchOrderByRows = false; // Search column by column

            // Найдите "abc" — должно вернуть A3 (строка 2, столбец 0) при поиске по столбцам
            Cell foundCell = worksheet.Cells.Find("abc", null, findOptions);

            // Вывести результат.
            Console.WriteLine($"Found 'abc' at row: {foundCell.Row}, column: {foundCell.Column}");
        }
    }
}
```

### См. также

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


