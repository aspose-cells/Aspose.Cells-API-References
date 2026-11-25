---
title: "MarkdownSaveOptions.MarkdownSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore MarkdownSaveOptions. Crea le opzioni per salvare un documento markdown"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/markdownsaveoptions/
---
## MarkdownSaveOptions constructor

Crea le opzioni per salvare il documento markdown

```csharp
public MarkdownSaveOptions()
```

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Dimostra il costruttore MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = Environment.NewLine
            };

            // Salva come Markdown
            workbook.Save("MarkdownOutput.md", saveOptions);

            Console.WriteLine("Markdown file created successfully.");
        }
    }
}
```

### Vedi anche

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


