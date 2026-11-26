---
title: "Cells.Ranges"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает коллекцию объектов Range, созданных во время выполнения"
type: docs
url: /ru/net/aspose.cells/cells/ranges/
---
## Cells.Ranges property

Получает коллекцию объектов [`Range`](../../range/) , созданных во время выполнения.

```csharp
public RangeCollection Ranges { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRangesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте и добавьте диапазон в коллекцию Ranges
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Вставьте строки и продемонстрируйте расширение диапазона
            worksheet.Cells.InsertRows(2, 2, true);
            
            Console.WriteLine($"Range row count after insertion: {cellRange.RowCount}");
        }
    }
}
```

### См. также

* class [RangeCollection](../../rangecollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


