---
title: "PaginatedSaveOptions.CheckWorkbookDefaultFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions‑egenskap. När tecken i Excel är Unicode och inte har korrekt teckensnitt i cellstilen kan de visas som block i pdfimage. Ställ in detta till true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken."
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/
---
## PaginatedSaveOptions.CheckWorkbookDefaultFont property

När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta på true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Anmärkningar

Standard är true.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Test Content");
            
            // Konfigurera PDF‑sparalternativ
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CheckWorkbookDefaultFont = false;
            
            // Spara till PDF
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF saved with CheckWorkbookDefaultFont set to false");
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


