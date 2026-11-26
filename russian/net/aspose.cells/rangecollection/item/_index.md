---
title: "RangeCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RangeCollection. Возвращает элемент Range по указанному индексу"
type: docs
url: /ru/net/aspose.cells/rangecollection/item/
---
## RangeCollection indexer

Возвращает элемент [`Range`](../../range/) по указанному индексу.

```csharp
public Range this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать несколько диапазонов
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");

            // Добавить диапазоны в коллекцию
            RangeCollection ranges = worksheet.Cells.Ranges;
            ranges.Add(range1);
            ranges.Add(range2);
            ranges.Add(range3);

            // Продемонстрировать использование свойства Item
            Console.WriteLine("Range Collection Count: " + ranges.Count);
            for (int i = 0; i < ranges.Count; i++)
            {
                Aspose.Cells.Range currentRange = ranges[i]; // Using Item property
                Console.WriteLine($"Range {i + 1}: {currentRange.Address}");
                Console.WriteLine($"  - FirstRow: {currentRange.FirstRow}");
                Console.WriteLine($"  - FirstColumn: {currentRange.FirstColumn}");
                Console.WriteLine($"  - RowCount: {currentRange.RowCount}");
                Console.WriteLine($"  - ColumnCount: {currentRange.ColumnCount}");
            }

            // Получить конкретный диапазон по индексу
            Aspose.Cells.Range secondRange = ranges[1]; // Using Item property
            Console.WriteLine("\nSecond range details:");
            Console.WriteLine($"Address: {secondRange.Address}");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


