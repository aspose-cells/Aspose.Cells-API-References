---
title: "PdfSaveOptions.EmbedStandardWindowsFonts"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. true för att bädda in TrueType-teckensnitt. Påverkar endast ASCII-tecken 32127. Teckensnitt för teckenkoder större än 127 bäddas alltid in. Teckensnitt bäddas alltid in för PDF/A1a PDF/A1b-standarden. Standard är true"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/
---
## PdfSaveOptions.EmbedStandardWindowsFonts property

Sant för att bädda in TrueType‑teckensnitt. Påverkar endast ASCII‑tecken 32‑127. Teckensnitt för teckenkoder över 127 bäddas alltid in. Teckensnitt bäddas alltid in för PDF/A-1a, PDF/A-1b‑standard. Standard är sant.

```csharp
public bool EmbedStandardWindowsFonts { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedStandardWindowsFontsDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF with embedded fonts");

            // Ange PDF-sparalternativ med EmbedStandardWindowsFonts-egenskap
            PdfSaveOptions options = new PdfSaveOptions();
            options.EmbedStandardWindowsFonts = true;

            // Spara till minnesström
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved with embedded fonts: " + (ms.Length > 0));
            }

            // Demonstrera inaktivering av teckensnitts-inbäddning
            options.EmbedStandardWindowsFonts = false;
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved without embedded fonts: " + (ms.Length > 0));
            }
        }
    }
}
```

### Se även

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


