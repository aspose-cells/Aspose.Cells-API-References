---
title: "MarkdownSaveOptions.Encoding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions-Eigenschaft. Liest und setzt die Standardkodierung"
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/encoding/
---
## MarkdownSaveOptions.Encoding property

Liest und setzt die Standardkodierung.

```csharp
public Encoding Encoding { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Markdown");

            // Konfigurieren Sie die Speicheroptionen mit UTF8-Kodierung
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8
            };

            // Speichern mit angegebener Kodierung
            workbook.Save("MarkdownWithEncoding.md", saveOptions);

            Console.WriteLine("Markdown file saved with UTF-8 encoding.");
        }
    }
}
```

### Siehe auch

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


