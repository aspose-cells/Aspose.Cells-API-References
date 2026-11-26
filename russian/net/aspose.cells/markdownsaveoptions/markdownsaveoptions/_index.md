---
title: "MarkdownSaveOptions.MarkdownSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор MarkdownSaveOptions. Создаёт параметры для сохранения markdown‑документа"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/markdownsaveoptions/
---
## MarkdownSaveOptions constructor

Создаёт параметры для сохранения markdown-документа

```csharp
public MarkdownSaveOptions()
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Продемонстрировать конструктор MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = Environment.NewLine
            };

            // Сохранить как Markdown
            workbook.Save("MarkdownOutput.md", saveOptions);

            Console.WriteLine("Markdown file created successfully.");
        }
    }
}
```

### См. также

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


