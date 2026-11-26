---
title: "Row.FirstDataCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Получает первую непустую ячейку в строке"
type: docs
url: /ru/net/aspose.cells/row/firstdatacell/
---
## Row.FirstDataCell property

Получает первую непустую ячейку в строке.

```csharp
public Cell FirstDataCell { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Поместите значения в разные ячейки
            cells["A1"].PutValue("Header");
            cells["B2"].PutValue("FirstData");
            cells["C2"].PutValue("SecondData");
            
            // Получить первую ячейку данных в строке 1 (индекс 0)
            Cell firstDataCellRow1 = cells.Rows[0].FirstDataCell;
            Console.WriteLine("First data cell in row 1: " + (firstDataCellRow1 != null ? firstDataCellRow1.Name : "null"));
            
            // Получить первую ячейку данных в строке 2 (индекс 1)
            Cell firstDataCellRow2 = cells.Rows[1].FirstDataCell;
            Console.WriteLine("First data cell in row 2: " + firstDataCellRow2.Name);
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


