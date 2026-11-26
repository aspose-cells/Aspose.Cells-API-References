---
title: "Row.Index"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Возвращает индекс этой строки"
type: docs
url: /ru/net/aspose.cells/row/index/
---
## Row.Index property

Получает индекс этой строки.

```csharp
public int Index { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Итерируйте строки и продемонстрируйте свойство Index
            foreach (Row row in worksheet.Cells.Rows)
            {
                Console.WriteLine($"Processing row with index: {row.Index}");
                if (row.Index > 0) // Skip header row
                {
                    Console.WriteLine($"Data in row {row.Index}: " +
                        $"{worksheet.Cells[row.Index, 0].StringValue}, " +
                        $"{worksheet.Cells[row.Index, 1].IntValue}");
                }
            }
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


