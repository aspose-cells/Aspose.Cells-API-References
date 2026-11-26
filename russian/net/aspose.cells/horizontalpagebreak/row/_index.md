---
title: "HorizontalPageBreak.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HorizontalPageBreak. Возвращает нулевой индекс строки"
type: docs
url: /ru/net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

Получает нулевой индекс строки.

```csharp
public int Row { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте горизонтальные разрывы страниц
            worksheet.HorizontalPageBreaks.Add(6);
            worksheet.HorizontalPageBreaks.Add(12);

            // Получите коллекцию горизонтальных разрывов страниц
            HorizontalPageBreakCollection breaks = worksheet.HorizontalPageBreaks;

            // Отобразите номера строк разрывов страниц
            Console.WriteLine("Page break at row: " + breaks[0].Row);
            Console.WriteLine("Page break at row: " + breaks[1].Row);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


