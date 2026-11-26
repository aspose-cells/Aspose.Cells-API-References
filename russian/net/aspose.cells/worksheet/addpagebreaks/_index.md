---
title: "Worksheet.AddPageBreaks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Добавляет разрыв страницы"
type: docs
url: /ru/net/aspose.cells/worksheet/addpagebreaks/
---
## Worksheet.AddPageBreaks method

Добавляет разрыв страницы.

```csharp
public void AddPageBreaks(string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String |  |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAddPageBreaksWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить горизонтальный разрыв страницы в строке 1 (B2)
            worksheet.AddPageBreaks("B2");

            // Добавить горизонтальный разрыв страницы в строке 9 (B10)
            worksheet.AddPageBreaks("B10");

            // Проверить, что первый разрыв страницы был добавлен в строке 1
            Console.WriteLine("First page break row: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


