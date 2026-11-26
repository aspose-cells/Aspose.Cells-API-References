---
title: "Range.Top"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Получает расстояние в пунктах от верхнего края строки 1 до верхнего края диапазона."
type: docs
url: /ru/net/aspose.cells/range/top/
---
## Range.Top property

Получает расстояние в пунктах от верхнего края строки 1 до верхнего края диапазона.

```csharp
public double Top { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyTopDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать диапазон и задать несколько значений.
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            range[0, 0].PutValue("Test");
            
            // Продемонстрировать использование свойства Top.
            Console.WriteLine("Range Top position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


