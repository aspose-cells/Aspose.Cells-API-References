---
title: "VerticalPageBreak.Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VerticalPageBreak. Получает индекс столбца вертикального разрыва страницы"
type: docs
url: /ru/net/aspose.cells/verticalpagebreak/column/
---
## VerticalPageBreak.Column property

Получает индекс столбца вертикального разрыва страницы.

```csharp
public int Column { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить вертикальные разрывы страниц в столбцах 4 и 8
            worksheet.VerticalPageBreaks.Add(4);
            worksheet.VerticalPageBreaks.Add(8);

            // Получить коллекцию вертикальных разрывов страниц
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;

            // Отобразить информацию о каждом вертикальном разрыве страницы
            Console.WriteLine("Vertical Page Breaks Count: " + vpagebreaks.Count);
            
            foreach (VerticalPageBreak vpagebreak in vpagebreaks)
            {
                Console.WriteLine("\nPage Break at Column: " + vpagebreak.Column);
                Console.WriteLine("Start Row: " + vpagebreak.StartRow);
                Console.WriteLine("End Row: " + vpagebreak.EndRow);
            }

            // Сохраните книгу
            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### См. также

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


