---
title: "ListObject.EndRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Возвращает конечную строку диапазона"
type: docs
url: /ru/net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

Получает конечную строку диапазона.

```csharp
public int EndRow { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Создать примерные данные
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B3"].PutValue(25);
            
            // Создать объект списка/таблицу
            int idx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[idx];
            
            // Отобразить начальное EndRow
            Console.WriteLine("Initial EndRow: " + table.EndRow);
            
            // Добавить новую строку в таблицу
            table.PutCellValue(4, 0, "Tom");
            table.PutCellValue(4, 1, 28);
            
            // Отобразить обновлённое EndRow
            Console.WriteLine("Updated EndRow: " + table.EndRow);
            
            // Сохраните книгу
            wb.Save("ListObjectEndRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


