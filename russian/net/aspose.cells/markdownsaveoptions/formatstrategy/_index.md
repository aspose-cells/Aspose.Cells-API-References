---
title: "MarkdownSaveOptions.FormatStrategy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MarkdownSaveOptions. Получает и задаёт стратегию форматирования при экспорте значения ячейки как строки"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/formatstrategy/
---
## MarkdownSaveOptions.FormatStrategy property

Получает и задает стратегию форматирования при экспорте значения ячейки как строки.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные с разными форматами
            worksheet.Cells["A1"].PutValue(123.456); // Numeric value
            worksheet.Cells["A2"].PutValue(DateTime.Now); // Date value
            worksheet.Cells["A3"].PutValue(true); // Boolean value

            // Создайте параметры сохранения Markdown с стратегией форматирования DisplayString
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString
            };

            // Сохраните книгу в формате Markdown
            workbook.Save("MarkdownWithDisplayString.md", saveOptions);

            // Перейдите к CellValueFormatStrategy.CellStyle
            saveOptions.FormatStrategy = CellValueFormatStrategy.CellStyle;
            workbook.Save("MarkdownWithCellStyle.md", saveOptions);

            Console.WriteLine("Markdown files saved successfully with different format strategies.");
        }
    }
}
```

### См. также

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


