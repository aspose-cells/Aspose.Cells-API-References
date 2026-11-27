---
title: "MarkdownSaveOptions.LineSeparator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions egenskap. Hämtar och anger radseparatorn"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/lineseparator/
---
## MarkdownSaveOptions.LineSeparator property

Hämtar och anger radseparatorn.

```csharp
public string LineSeparator { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Value1");
            worksheet.Cells["B2"].PutValue("Value2");

            // Konfigurera Markdown-sparalternativ med anpassad radseparator
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                LineSeparator = "\n", // Using Unix-style line endings
                Encoding = Encoding.UTF8
            };

            // Spara som Markdown‑fil
            workbook.Save("MarkdownWithLineSeparator.md", saveOptions);

            Console.WriteLine("Markdown file saved with custom line separator.");
        }
    }
}
```

### Se även

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


