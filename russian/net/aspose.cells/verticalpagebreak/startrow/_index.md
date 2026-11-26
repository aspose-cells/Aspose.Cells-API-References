---
title: "VerticalPageBreak.StartRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VerticalPageBreak. Получает индекс начальной строки вертикального разрыва страницы"
type: docs
url: /ru/net/aspose.cells/verticalpagebreak/startrow/
---
## VerticalPageBreak.StartRow property

Получает индекс начальной строки вертикального разрыва страницы.

```csharp
public int StartRow { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyStartRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Изначально добавить вертикальные разрывы страниц с желаемой начальной строкой (2)
            worksheet.VerticalPageBreaks.Add(2, 0, 10);
            VerticalPageBreak vPageBreak = worksheet.VerticalPageBreaks[0];

            // Отобразить свойство StartRow
            Console.WriteLine("Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Поскольку StartRow только для чтения, нам нужно удалить и добавить заново, чтобы изменить его
            worksheet.VerticalPageBreaks.RemoveAt(0);
            worksheet.VerticalPageBreaks.Add(5, 0, 10);
            vPageBreak = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Modified Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Сохраните книгу
            workbook.Save("VerticalPageBreakExample.xlsx");
        }
    }
}
```

### См. также

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


