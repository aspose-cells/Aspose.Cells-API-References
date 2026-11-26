---
title: "Класс Top10Filter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Top10Filter. Представляет верхние N процентов или количество элементов для фильтрации."
type: docs
url: /ru/net/aspose.cells/top10filter/
---
## Top10Filter class

Представляет верхние N (процент или количество элементов) для фильтрации.

```csharp
public class Top10Filter
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } | (**Obsolete.**) Фактическое значение ячейки в диапазоне, которое используется для выполнения сравнения для этого фильтра. Это кэшированное значение во время процесса обновления. |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | Указывает, следует ли фильтровать по процентному значению столбца |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | Указывает, следует ли фильтровать по верхнему порядку |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | Получает и задает верхнее или нижнее значение, используемое в качестве критерия фильтра. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTop10FilterDemo
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
                worksheet.Cells["C" + i].PutValue("Item " + (i-6));
            }
            
            // Примените автофильтр и фильтр Top 10
            worksheet.AutoFilter.Range = "B6:C16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5); // Filter top 5 values in column B
            
            // Получите Top10Filter и проверьте его свойства
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent);
            Console.WriteLine("Items: " + filter.Items);
            
            // Обновите фильтр и проверьте скрытые строки
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
            
            // Сохраните книгу
            workbook.Save("Top10FilterDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


