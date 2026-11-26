---
title: "Range.Intersect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Возвращает объект Range, представляющий прямоугольное пересечение двух диапазонов"
type: docs
url: /ru/net/aspose.cells/range/intersect/
---
## Range.Intersect method

Возвращает объект [`Range`](../), представляющий прямоугольное пересечение двух диапазонов.

```csharp
public Range Intersect(Range range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | Диапазон | Пересекающийся диапазон. |

### Возвращаемое значение

Возвращает объект [`Range`](../)

### Примечания

Если два диапазона не пересекаются, возвращает null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIntersectWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            Aspose.Cells.Range range1 = cells.CreateRange("A1:A5");
            Aspose.Cells.Range range2 = cells.CreateRange("A3:A10");
            
            Aspose.Cells.Range intersectRange = range1.Intersect(range2);
            
            Console.WriteLine("Intersected range: " + intersectRange.Address);
            workbook.Save("IntersectDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


