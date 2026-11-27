---
title: "PdfBookmarkEntry.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfBookmarkEntry-egenskap. Titel för ett bokmärke"
type: docs
url: /sv/net/aspose.cells.rendering/pdfbookmarkentry/text/
---
## PdfBookmarkEntry.Text property

Titel för ett bokmärke.

```csharp
public string Text { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempelinnehåll
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // Skapa PDF-bokmärkespost
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "Section 1"; // Demonstrating Text property usage
            entry.Destination = worksheet.Cells["A1"];
            entry.IsOpen = true;
            
            // Ställ in sparalternativ med bokmärke
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.Bookmark = entry;
            
            // Spara arbetsboken med bokmärke
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF with bookmark created successfully.");
        }
    }
}
```

### Se även

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


