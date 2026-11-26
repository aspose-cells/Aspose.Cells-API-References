---
title: "ListObject.StartColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Возвращает начальный столбец диапазона"
type: docs
url: /ru/net/aspose.cells.tables/listobject/startcolumn/
---
## ListObject.StartColumn property

Получает начальный столбец диапазона.

```csharp
public int StartColumn { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyStartColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать примерные данные для таблицы
            worksheet.Cells["E5"].PutValue("ID");
            worksheet.Cells["F5"].PutValue("Name");
            worksheet.Cells["G5"].PutValue("Age");
            
            worksheet.Cells["E6"].PutValue(1);
            worksheet.Cells["F6"].PutValue("John");
            worksheet.Cells["G6"].PutValue(30);
            
            worksheet.Cells["E7"].PutValue(2);
            worksheet.Cells["F7"].PutValue("Alice");
            worksheet.Cells["G7"].PutValue(25);

            // Создайте объект списка (таблица)
            int startRow = 5;
            int startCol = 4; // Column E (0-based index 4)
            int endRow = 7;
            int endCol = 6; // Column G (0-based index 6)
            
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(startRow, startCol, endRow, endCol, true)];
            
            // Продемонстрировать свойство StartColumn
            Console.WriteLine("Table starts at column index: " + table.StartColumn);
            Console.WriteLine("Table starts at column letter: " + CellsHelper.ColumnIndexToName(table.StartColumn));
            
            // Сохраните книгу
            workbook.Save("ListObjectStartColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


