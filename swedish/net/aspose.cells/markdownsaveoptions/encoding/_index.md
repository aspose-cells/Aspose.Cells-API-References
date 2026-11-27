---
title: "MarkdownSaveOptions.Encoding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions egenskap. Hämtar och anger standardkodningen"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/encoding/
---
## MarkdownSaveOptions.Encoding property

Hämtar och anger standardkodningen.

```csharp
public Encoding Encoding { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Markdown");

            // Konfigurera sparalternativ med UTF8-kodning
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8
            };

            // Spara med angiven kodning
            workbook.Save("MarkdownWithEncoding.md", saveOptions);

            Console.WriteLine("Markdown file saved with UTF-8 encoding.");
        }
    }
}
```

### Se även

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


