---
title: "Row.FirstCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Возвращает объект первой ячейки в строке"
type: docs
url: /ru/net/aspose.cells/row/firstcell/
---
## Row.FirstCell property

Получает первый объект ячейки в строке.

```csharp
public Cell FirstCell { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить данные в ячейки первой строки
            worksheet.Cells["A1"].PutValue("First Cell");
            worksheet.Cells["B1"].PutValue("Second Cell");
            worksheet.Cells["C1"].PutValue("Third Cell");
            
            // Получить первую строку
            Row row = worksheet.Cells.Rows[0];
            
            // Продемонстрировать свойство FirstCell
            Cell firstCell = row.FirstCell;
            Console.WriteLine("First cell in row: " + firstCell.Name + " with value: " + firstCell.StringValue);
            
            // Изменить первую ячейку
            firstCell.PutValue("Modified First Cell");
            Console.WriteLine("Updated first cell value: " + firstCell.StringValue);
            
            // Сохраните книгу
            workbook.Save("RowFirstCellDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


