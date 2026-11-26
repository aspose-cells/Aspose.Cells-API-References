---
title: "Cells.CountLarge"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Возвращает общее количество созданных объектов Cell"
type: docs
url: /ru/net/aspose.cells/cells/countlarge/
---
## Cells.CountLarge property

Получает общее количество созданных объектов Cell.

```csharp
public long CountLarge { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyCountLargeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B2"].PutValue("World");
            worksheet.Cells["C3"].PutValue(123);
            
            // Продемонстрировать свойство CountLarge
            long cellCount = worksheet.Cells.CountLarge;
            Console.WriteLine($"Total cells in worksheet: {cellCount}");
            
            // Показать размер бумаги для демонстрации
            Console.WriteLine($"Paper Height: {worksheet.PageSetup.PaperHeight}");
            Console.WriteLine($"Paper Width: {worksheet.PageSetup.PaperWidth}");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


