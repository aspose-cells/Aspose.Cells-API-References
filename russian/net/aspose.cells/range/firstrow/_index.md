---
title: "Range.FirstRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает индекс первой строки диапазона"
type: docs
url: /ru/net/aspose.cells/range/firstrow/
---
## Range.FirstRow property

Получает индекс первой строки диапазона.

```csharp
public int FirstRow { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и получите доступ к первому рабочему листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми данными
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Создайте диапазон
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Получите и отобразите свойство FirstRow
            Console.WriteLine("First row index of range: " + range.FirstRow);

            // Получите первую ячейку в первой строке диапазона
            Cell firstCell = worksheet.Cells[range.FirstRow, range.FirstColumn];
            Console.WriteLine("First cell value: " + firstCell.StringValue);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


