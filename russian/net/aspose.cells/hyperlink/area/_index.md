---
title: "Hyperlink.Area"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Hyperlink. Возвращает диапазон гиперссылки"
type: docs
url: /ru/net/aspose.cells/hyperlink/area/
---
## Hyperlink.Area property

Получает диапазон гиперссылки.

```csharp
public CellArea Area { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Main Menu");
            worksheet.Cells["A3"].PutValue("Chapter 1");
            worksheet.Cells["A4"].PutValue("Chapter 2");
            
            // Добавить гиперссылки
            int hyperlinkIndex1 = worksheet.Hyperlinks.Add("A3", 1, 1, "Sheet2!A1");
            int hyperlinkIndex2 = worksheet.Hyperlinks.Add("A4", 1, 1, "Sheet3!A1");

            // Получить гиперссылки и продемонстрировать использование свойства Area
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            string chapter2Address = "";
            foreach (Hyperlink link in hyperlinks)
            {
                // Проверить, находится ли гиперссылка в ячейке A4 с помощью свойства Area
                if (link.Area.StartRow == 3 && link.Area.StartColumn == 0)
                {
                    chapter2Address = link.Address;
                    break;
                }
            }

            Console.WriteLine("Chapter 2 hyperlink address: " + chapter2Address);
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


