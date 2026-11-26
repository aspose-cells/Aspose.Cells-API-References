---
title: "Класс HorizontalPageBreak"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.HorizontalPageBreak. Инкапсулирует объект, представляющий горизонтальный разрыв страницы"
type: docs
url: /ru/net/aspose.cells/horizontalpagebreak/
---
## HorizontalPageBreak class

Инкапсулирует объект, представляющий горизонтальный разрыв страницы.

```csharp
public class HorizontalPageBreak
```

## Свойства

| Имя | Описание |
| --- | --- |
| [EndColumn](../../aspose.cells/horizontalpagebreak/endcolumn/) { get; } | Получает индекс конечного столбца этого горизонтального разрыва страницы. |
| [Row](../../aspose.cells/horizontalpagebreak/row/) { get; } | Получает нулевой индекс строки. |
| [StartColumn](../../aspose.cells/horizontalpagebreak/startcolumn/) { get; } | Получает индекс начального столбца этого горизонтального разрыва страницы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakDemo
    {
        public static void HorizontalPageBreakExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            
            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте разрыв страницы в ячейку Y30
            int index = worksheet.HorizontalPageBreaks.Add("Y30");
            
            // Получите недавно добавленный горизонтальный разрыв страницы
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
            
            // Отобразите свойства горизонтального разрыва страницы
            Console.WriteLine("Horizontal Page Break Details:");
            Console.WriteLine($"Row: {hPageBreak.Row}");
            Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
            Console.WriteLine($"End Column: {hPageBreak.EndColumn}");
            
            // Сохраните книгу
            workbook.Save("HorizontalPageBreakExample.xlsx");
            workbook.Save("HorizontalPageBreakExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


