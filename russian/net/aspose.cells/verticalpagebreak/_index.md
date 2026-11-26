---
title: "Класс VerticalPageBreak"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.VerticalPageBreak. Инкапсулирует объект, представляющий вертикальный разрыв страницы"
type: docs
url: /ru/net/aspose.cells/verticalpagebreak/
---
## VerticalPageBreak class

Инкапсулирует объект, представляющий вертикальный разрыв страницы.

```csharp
public class VerticalPageBreak
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column/) { get; } | Получает индекс столбца вертикального разрыва страницы. |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow/) { get; } | Получает индекс конечной строки вертикального разрыва страницы. |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow/) { get; } | Получает индекс начальной строки вертикального разрыва страницы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakDemo
    {
        public static void VerticalPageBreakExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу в рабочей книге
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить вертикальный разрыв страницы в столбце G (индекс 6)
            worksheet.VerticalPageBreaks.Add("G5");

            // Сохраните книгу
            workbook.Save("VerticalPageBreakExample.xlsx");

            // Получить доступ к добавленному вертикальному разрыву страницы
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // Отобразить свойства вертикального разрыва страницы
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


