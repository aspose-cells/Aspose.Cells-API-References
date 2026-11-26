---
title: "Top10Filter.IsTop"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Top10Filter. Указывает, следует ли фильтровать по верхнему порядку"
type: docs
url: /ru/net/aspose.cells/top10filter/istop/
---
## Top10Filter.IsTop property

Указывает, следует ли фильтровать по верхнему порядку

```csharp
public bool IsTop { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsTopDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["B6"].PutValue("Value");
            for (int i = 7; i <= 16; i++)
            {
                worksheet.Cells["B" + i].PutValue(20 - i);
            }

            // Применить фильтр top 5
            worksheet.AutoFilter.Range = "B6:B16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Получить фильтр и проверить свойство IsTop
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop); // Should output "True"
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output "False"
            
            // Обновить фильтр и проверить скрытые строки
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### См. также

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


