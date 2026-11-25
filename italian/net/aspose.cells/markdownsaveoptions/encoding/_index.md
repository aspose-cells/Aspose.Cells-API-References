---
title: "MarkdownSaveOptions.Encoding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Ottiene e imposta la codifica predefinita"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/encoding/
---
## MarkdownSaveOptions.Encoding property

Ottiene e imposta la codifica predefinita.

```csharp
public Encoding Encoding { get; set; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Markdown");

            // Configura le opzioni di salvataggio con codifica UTF8
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8
            };

            // Salva con la codifica specificata
            workbook.Save("MarkdownWithEncoding.md", saveOptions);

            Console.WriteLine("Markdown file saved with UTF-8 encoding.");
        }
    }
}
```

### Vedi anche

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


