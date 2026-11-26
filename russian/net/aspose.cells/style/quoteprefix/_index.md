---
title: "Style.QuotePrefix"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Указывает, начинается ли значение ячейки с одинарной кавычки"
type: docs
url: /ru/net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

Указывает, начинается ли значение ячейки с одинарной кавычки.

```csharp
public bool QuotePrefix { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к ячейке B10 и установите её значение
            Cell cell = worksheet.Cells["B10"];
            cell.PutValue("'12345"); // Note the single quote prefix

            // Получить стиль ячейки и включить QuotePrefix
            Style style = cell.GetStyle();
            style.QuotePrefix = true;
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Проверить свойство QuotePrefix
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cell loadedCell = loadedWorkbook.Worksheets[0].Cells["B10"];
            Console.WriteLine("QuotePrefix is set: " + loadedCell.GetStyle().QuotePrefix);
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


