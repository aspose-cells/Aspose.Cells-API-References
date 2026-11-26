---
title: "Range.Height"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает ширину диапазона в пунктах"
type: docs
url: /ru/net/aspose.cells/range/height/
---
## Range.Height property

Получает ширину диапазона в пунктах.

```csharp
public double Height { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить высоту строк для демонстрации
            worksheet.Cells.SetRowHeight(1, 15.0); // Row 2 (0-based index 1)
            worksheet.Cells.SetRowHeight(2, 20.0); // Row 3
            worksheet.Cells.SetRowHeight(3, 25.0); // Row 4

            // Создать диапазон, охватывающий строки 2‑4 (B2:C4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Продемонстрировать свойство Height
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Calculated Height (sum of row heights): " + 
                (worksheet.Cells.GetRowHeight(1) + 
                 worksheet.Cells.GetRowHeight(2) + 
                 worksheet.Cells.GetRowHeight(3)));
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


