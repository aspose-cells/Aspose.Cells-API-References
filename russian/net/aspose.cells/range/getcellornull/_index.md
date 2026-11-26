---
title: "Range.GetCellOrNull"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Получает объект Cell или null в этом диапазоне"
type: docs
url: /ru/net/aspose.cells/range/getcellornull/
---
## Range.GetCellOrNull method

Получает объект [`Cell`](../../cell/) или null в этом диапазоне.

```csharp
public Cell GetCellOrNull(int rowOffset, int columnOffset)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | Int32 | Смещение строки в этом диапазоне, начиная с нуля. |
| columnOffset | Int32 | Смещение столбца в этом диапазоне, начиная с нуля. |

### Возвращаемое значение

[`Cell`](../../cell/) object.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetCellOrNullWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте диапазон
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            
            // Заполните диапазон данными
            range[0, 0].PutValue("Cell A1");
            range[0, 1].PutValue("Cell B1");
            range[1, 0].PutValue("Cell A2");
            
            // Продемонстрируйте GetCellOrNull с параметрами Int32
            Cell cell1 = range.GetCellOrNull(0, 0);
            Console.WriteLine("Cell (0,0): " + (cell1 != null ? cell1.StringValue : "null"));
            
            Cell cell2 = range.GetCellOrNull(1, 1);
            Console.WriteLine("Cell (1,1): " + (cell2 != null ? cell2.StringValue : "null"));
            
            // Попробуйте получить ячейку за пределами диапазона (должно вернуть null)
            Cell cell3 = range.GetCellOrNull(2, 0);
            Console.WriteLine("Cell (2,0): " + (cell3 != null ? cell3.StringValue : "null"));
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


