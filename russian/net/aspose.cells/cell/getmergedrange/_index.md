---
title: "Cell.GetMergedRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Возвращает объект Range, который представляет объединённый диапазон"
type: docs
url: /ru/net/aspose.cells/cell/getmergedrange/
---
## Cell.GetMergedRange method

Возвращает объект [`Range`](../../range/), который представляет объединённый диапазон.

```csharp
public Range GetMergedRange()
```

### Возвращаемое значение

[`Range`](../../range/) object. Null if this cell is not merged.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetMergedRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Объединить ячейки
            cells.Merge(0, 0, 2, 2);

            // Получить первую ячейку
            Cell cell = cells[0, 0];

            // Получить информацию об объединённом диапазоне
            Aspose.Cells.Range mergedRange = cell.GetMergedRange();
            
            // Вывести детали объединённого диапазона
            Console.WriteLine("Merged Range Details:");
            Console.WriteLine($"First Row: {mergedRange.FirstRow}");
            Console.WriteLine($"First Column: {mergedRange.FirstColumn}");
            Console.WriteLine($"Row Count: {mergedRange.RowCount}");
            Console.WriteLine($"Column Count: {mergedRange.ColumnCount}");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


