---
title: "Range.GetOffset"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Возвращает диапазон Range по смещению"
type: docs
url: /ru/net/aspose.cells/range/getoffset/
---
## Range.GetOffset method

Возвращает диапазон [`Range`](../) по смещению.

```csharp
public Range GetOffset(int rowOffset, int columnOffset)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | Int32 | Смещение строки в этом диапазоне, начиная с нуля. |
| columnOffset | Int32 | Смещение столбца в этом диапазоне, начиная с нуля. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetOffsetWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Создайте начальный диапазон
            Aspose.Cells.Range originalRange = cells.CreateRange("A1");
            Console.WriteLine("Original Range Address: " + originalRange.Address);
            
            // Получите диапазон со смещением
            Aspose.Cells.Range offsetRange = originalRange.GetOffset(1, 1);
            Console.WriteLine("Offset Range Address: " + offsetRange.Address);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


