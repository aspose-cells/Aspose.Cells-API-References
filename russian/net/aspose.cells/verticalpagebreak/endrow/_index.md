---
title: "VerticalPageBreak.EndRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VerticalPageBreak. Получает индекс конечной строки вертикального разрыва страницы"
type: docs
url: /ru/net/aspose.cells/verticalpagebreak/endrow/
---
## VerticalPageBreak.EndRow property

Получает индекс конечной строки вертикального разрыва страницы.

```csharp
public int EndRow { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyEndRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить вертикальный разрыв страницы, охватывающий строки с 3 по 8 в столбце C (индекс 2)
            worksheet.VerticalPageBreaks.Add("C3:C8");

            // Получить первый вертикальный разрыв страницы
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            
            // Отобразить конечную строку разрыва страницы
            Console.WriteLine("Vertical Page Break End Row: " + vpb.EndRow);
            
            // Поскольку EndRow только для чтения, мы продемонстрируем получение значения, но не его установку
            // Следующая строка удалена, так как вызывает ошибку компиляции:
            // vpb.EndRow = 10;
            
            // Вместо этого мы добавим другой разрыв страницы с другим значением конечной строки
            worksheet.VerticalPageBreaks.Add("C3:C10");
            VerticalPageBreak vpb2 = worksheet.VerticalPageBreaks[1];
            Console.WriteLine("Second Page Break End Row: " + vpb2.EndRow);
        }
    }
}
```

### См. также

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


