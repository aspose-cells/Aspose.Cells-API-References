---
title: "Range.FirstColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает индекс первого столбца диапазона"
type: docs
url: /ru/net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

Получает индекс первого столбца диапазона.

```csharp
public int FirstColumn { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Создайте диапазон
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");

            // Продемонстрировать свойство FirstColumn
            Console.WriteLine("First column index of range: " + range.FirstColumn);

            // Использовать FirstColumn для доступа к ячейкам в первом столбце диапазона
            for (int i = 0; i < range.RowCount; i++)
            {
                Cell cell = range[i, 0]; // Access first column (index 0) of the range
                Console.WriteLine($"Cell[{i},0] value: {cell.StringValue}");
            }

            // Сохраните книгу
            workbook.Save("RangeFirstColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


