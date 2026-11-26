---
title: "UnionRange.Ranges"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnionRange. Возвращает все объединённые диапазоны"
type: docs
url: /ru/net/aspose.cells/unionrange/ranges/
---
## UnionRange.Ranges property

Получает все объединённые диапазоны.

```csharp
public Range[] Ranges { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyRangesDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            Aspose.Cells.Range r1 = cells.CreateRange("B1:C10");
            Aspose.Cells.Range r2 = cells.CreateRange("C2:D10");
            
            UnionRange unionRange = r1.UnionRanges(new Aspose.Cells.Range[] { r2 });
            
            Console.WriteLine("UnionRange contains {0} ranges:", unionRange.RangeCount);
            for (int i = 0; i < unionRange.RangeCount; i++)
            {
                Console.WriteLine("Range {0}: {1}", i + 1, unionRange.Ranges[i].Address);
            }
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


