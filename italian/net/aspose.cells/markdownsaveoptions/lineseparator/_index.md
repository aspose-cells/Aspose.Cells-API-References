---
title: "MarkdownSaveOptions.LineSeparator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Ottiene e imposta il separatore di riga"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/lineseparator/
---
## MarkdownSaveOptions.LineSeparator property

Ottiene e imposta il separatore di riga.

```csharp
public string LineSeparator { get; set; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyLineSeparatorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Value1");
            worksheet.Cells["B2"].PutValue("Value2");

            // Configura le opzioni di salvataggio Markdown con un separatore di riga personalizzato
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                LineSeparator = "\n", // Using Unix-style line endings
                Encoding = Encoding.UTF8
            };

            // Salva come file Markdown
            workbook.Save("MarkdownWithLineSeparator.md", saveOptions);

            Console.WriteLine("Markdown file saved with custom line separator.");
        }
    }
}
```

### Vedi anche

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


