---
title: "Range.Width"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает ширину диапазона в пунктах"
type: docs
url: /ru/net/aspose.cells/range/width/
---
## Range.Width property

Получает ширину диапазона в пунктах.

```csharp
public double Width { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить ширины столбцов для демонстрации свойства Width
            worksheet.Cells.SetColumnWidth(1, 20); // Column B width = 20
            worksheet.Cells.SetColumnWidth(2, 30); // Column C width = 30
            
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Отобразить ширину диапазона (сумма ширин столбцов в диапазоне)
            Console.WriteLine("Range Width: " + range.Width);
            
            // Отобразить отдельные свойства для проверки
            Console.WriteLine("Range Left Position: " + range.Left);
            Console.WriteLine("Range Top Position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


