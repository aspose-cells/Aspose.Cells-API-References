---
title: "Range.Left"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает расстояние в пунктах от левого края колонки A до левого края диапазона"
type: docs
url: /ru/net/aspose.cells/range/left/
---
## Range.Left property

Получает расстояние в пунктах от левого края столбца A до левого края диапазона.

```csharp
public double Left { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте диапазон от B2 до C4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Продемонстрировать использование свойства Left
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
            
            // Вычислить ожидаемые значения на основе тестового случая
            double expectedLeft = 64 / 96.0 * 72;
            Console.WriteLine("Expected Left position: " + expectedLeft);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


