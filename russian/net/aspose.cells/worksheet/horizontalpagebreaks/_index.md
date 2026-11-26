---
title: "Worksheet.HorizontalPageBreaks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает коллекцию HorizontalPageBreakCollection"
type: docs
url: /ru/net/aspose.cells/worksheet/horizontalpagebreaks/
---
## Worksheet.HorizontalPageBreaks property

Получает коллекцию [`HorizontalPageBreakCollection`](../../horizontalpagebreakcollection/).

```csharp
public HorizontalPageBreakCollection HorizontalPageBreaks { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте горизонтальные разрывы страниц разными способами
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            worksheet.HorizontalPageBreaks.Add(15, 2);
            worksheet.HorizontalPageBreaks.Add("G5");

            // Удалите первый разрыв страницы
            worksheet.HorizontalPageBreaks.RemoveAt(0);

            // Сохраните результаты
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
            workbook.Save("HorizontalPageBreaksDemo.pdf");
        }
    }
}
```

### См. также

* class [HorizontalPageBreakCollection](../../horizontalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


