---
title: "Row.LastCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Возвращает объект последней ячейки в строке"
type: docs
url: /ru/net/aspose.cells/row/lastcell/
---
## Row.LastCell property

Получает последний объект ячейки в строке.

```csharp
public Cell LastCell { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("First");
            worksheet.Cells["B1"].PutValue("Second");
            worksheet.Cells["C1"].PutValue("Last");

            // Получить первую строку
            Row row = worksheet.Cells.Rows[0];

            // Получить доступ к последней ячейке в строке
            Cell lastCell = row.LastCell;
            
            // Вывести значение последней ячейки
            Console.WriteLine("Last cell value: " + lastCell.Value);
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


