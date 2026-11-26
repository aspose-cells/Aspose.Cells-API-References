---
title: "HorizontalPageBreak.StartColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HorizontalPageBreak. Возвращает индекс начального столбца этого горизонтального разрыва страницы"
type: docs
url: /ru/net/aspose.cells/horizontalpagebreak/startcolumn/
---
## HorizontalPageBreak.StartColumn property

Получает индекс начального столбца этого горизонтального разрыва страницы.

```csharp
public int StartColumn { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyStartColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте разрывы страниц в разных столбцах, чтобы продемонстрировать StartColumn
            int index1 = worksheet.HorizontalPageBreaks.Add("Y30");
            int index2 = worksheet.HorizontalPageBreaks.Add("B30");
            
            HorizontalPageBreak hPageBreak1 = worksheet.HorizontalPageBreaks[index1];
            HorizontalPageBreak hPageBreak2 = worksheet.HorizontalPageBreaks[index2];
            
            Console.WriteLine($"First Break Start Column: {hPageBreak1.StartColumn}");
            Console.WriteLine($"Second Break Start Column: {hPageBreak2.StartColumn}");
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### См. также

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


