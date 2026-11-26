---
title: "Row.LastDataCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Возвращает последнюю непустую ячейку в строке"
type: docs
url: /ru/net/aspose.cells/row/lastdatacell/
---
## Row.LastDataCell property

Получает последнюю непустую ячейку в строке.

```csharp
public Cell LastDataCell { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Поместить данные в ячейки
            cells["A1"].PutValue("First cell");
            cells["B1"].PutValue("Second cell");
            cells["C2"].PutValue("Not in first row");
            
            // Получить последнюю ячейку с данными в первой строке
            Cell lastDataCell = cells.Rows[0].LastDataCell;
            
            Console.WriteLine("Last data cell in first row: " + lastDataCell.Name);
            Console.WriteLine("Value in last data cell: " + lastDataCell.StringValue);
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


