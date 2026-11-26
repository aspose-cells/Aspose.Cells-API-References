---
title: "HorizontalPageBreak.EndColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HorizontalPageBreak. Возвращает индекс конечного столбца этого горизонтального разрыва страницы"
type: docs
url: /ru/net/aspose.cells/horizontalpagebreak/endcolumn/
---
## HorizontalPageBreak.EndColumn property

Получает индекс конечного столбца этого горизонтального разрыва страницы.

```csharp
public int EndColumn { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте горизонтальный разрыв страницы в строке 5, охватывающий столбцы с 2 по 4
            int index = worksheet.HorizontalPageBreaks.Add(5, 2, 4);
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];

            // Отобразите свойство EndColumn
            Console.WriteLine("Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);

            // Поскольку EndColumn только для чтения, нам нужно удалить и заново добавить разрыв страницы, чтобы изменить его
            worksheet.HorizontalPageBreaks.RemoveAt(index);
            index = worksheet.HorizontalPageBreaks.Add(5, 2, 6);
            hPageBreak = worksheet.HorizontalPageBreaks[index];
            Console.WriteLine("Modified Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);
        }
    }
}
```

### См. также

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


