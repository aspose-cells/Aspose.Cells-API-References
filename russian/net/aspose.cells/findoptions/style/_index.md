---
title: "FindOptions.Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Формат для поиска"
type: docs
url: /ru/net/aspose.cells/findoptions/style/
---
## FindOptions.Style property

Формат для поиска.

```csharp
public Style Style { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль с синим шрифтом
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Blue;

            // Примените стиль к ячейке F2
            Cell cell = worksheet.Cells["F2"];
            cell.PutValue("SearchTarget");
            cell.SetStyle(style);

            // Создайте параметры поиска со стилем
            FindOptions options = new FindOptions();
            options.Style = style;

            // Найдите ячейку с соответствующим стилем
            Cell foundCell = worksheet.Cells.Find(null, null, options);

            // Выведите имя найденной ячейки
            Console.WriteLine("Cell found with matching style: " + foundCell?.Name);
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


