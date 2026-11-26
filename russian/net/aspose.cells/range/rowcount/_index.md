---
title: "Range.RowCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает количество строк в диапазоне"
type: docs
url: /ru/net/aspose.cells/range/rowcount/
---
## Range.RowCount property

Получает количество строк в диапазоне.

```csharp
public int RowCount { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте примерные данные в ячейках A1:B10
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row{row + 1}Col{col + 1}";
                }
            }

            // Создайте именованный диапазон, охватывающий A1:B10
            worksheet.Cells.CreateRange("A1", "B10").Name = "testRange";
            
            // Получить именованный диапазон
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
            
            // Продемонстрировать свойство RowCount
            Console.WriteLine($"Range starts at row: {range.FirstRow}");
            Console.WriteLine($"Range row count: {range.RowCount}");
            Console.WriteLine($"Range starts at column: {range.FirstColumn}");
            Console.WriteLine($"Range column count: {range.ColumnCount}");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


