---
title: "MarkdownSaveOptions.MarkdownSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions-konstruktor. Skapar alternativ för att spara markdown-dokument"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/markdownsaveoptions/
---
## MarkdownSaveOptions constructor

Skapar alternativ för att spara markdown‑dokument

```csharp
public MarkdownSaveOptions()
```

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Demonstrera MarkdownSaveOptions-konstruktor
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = Environment.NewLine
            };

            // Spara som Markdown
            workbook.Save("MarkdownOutput.md", saveOptions);

            Console.WriteLine("Markdown file created successfully.");
        }
    }
}
```

### Se även

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


