---
title: "PaginatedSaveOptions.DefaultFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions egenskap. När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdfimage. Ange DefaultFont såsom MingLiu eller MS Gothic för att visa dessa tecken. Om denna egenskap inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/defaultfont/
---
## PaginatedSaveOptions.DefaultFont property

När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är angiven kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode‑tecken.

```csharp
public string DefaultFont { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("This text will use the default font");
            worksheet.Cells["A2"].PutValue("如果默认字体支持中文，这将显示正确");

            // Konfigurera PDF-sparalternativ med standardteckensnitt
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultFont = "宋体";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;

            // Spara till PDF
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


