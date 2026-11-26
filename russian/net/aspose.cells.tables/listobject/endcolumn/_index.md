---
title: "ListObject.EndColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Получает конечный столбец диапазона"
type: docs
url: /ru/net/aspose.cells.tables/listobject/endcolumn/
---
## ListObject.EndColumn property

Получает конечный столбец диапазона.

```csharp
public int EndColumn { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Age");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i-1);
                worksheet.Cells[$"B{i}"].PutValue($"Person {i-1}");
                worksheet.Cells[$"C{i}"].PutValue(20 + i);
            }

            // Создать объект/таблицу списка
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 4, 2, true);
            ListObject table = worksheet.ListObjects[listObjectIndex];
            table.ShowTotals = true;
            
            // Отобразить исходный конечный столбец
            Console.WriteLine($"Original EndColumn: {table.EndColumn}");
            
            // Изменить размер таблицы, чтобы добавить ещё один столбец
            table.Resize(table.StartRow, table.StartColumn, table.EndRow, table.EndColumn + 1, table.ShowHeaderRow);
            
            // Отобразить новый конечный столбец
            Console.WriteLine($"New EndColumn: {table.EndColumn}");
            
            // Сохраните книгу
            workbook.Save("ListObjectEndColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


