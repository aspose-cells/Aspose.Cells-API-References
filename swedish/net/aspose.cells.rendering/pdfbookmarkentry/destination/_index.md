---
title: "PdfBookmarkEntry.Destination"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfBookmarkEntry-egenskap. Cellen som bokmärkeslänken pekar på"
type: docs
url: /sv/net/aspose.cells.rendering/pdfbookmarkentry/destination/
---
## PdfBookmarkEntry.Destination property

Cellen som bokmärkeslänken pekar på.

```csharp
public Cell Destination { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyDestinationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempelinnehåll
            worksheet.Cells["A1"].PutValue("Bookmark Destination");
            
            // Konfigurera PDF-sparalternativ med bokmärke
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "Sample Bookmark";
            entry.Destination = worksheet.Cells["A1"]; // Demonstrate Destination property
            entry.IsOpen = true;
            
            pdfSaveOptions.Bookmark = entry;
            
            // Spara PDF-filen
            workbook.Save("PdfBookmarkEntryPropertyDestinationDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* class [Cell](../../../aspose.cells/cell/)
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


