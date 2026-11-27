---
title: "PdfSaveOptions.Bookmark"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. Hämtar och anger PdfBookmarkEntry‑objektet"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/bookmark/
---
## PdfSaveOptions.Bookmark property

Hämtar och anger [`PdfBookmarkEntry`](../../../aspose.cells.rendering/pdfbookmarkentry/)‑objektet.

```csharp
public PdfBookmarkEntry Bookmark { get; set; }
```

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyBookmarkDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till tre kalkylblad
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            Worksheet sheet3 = workbook.Worksheets.Add("Sheet3");

            // Ställ in värden i celler som kommer att vara bokmärkesdestinationer
            sheet1.Cells["A1"].Value = "Sheet1 Content";
            sheet2.Cells["A1"].Value = "Sheet2 Content";
            sheet3.Cells["A1"].Value = "Sheet3 Content";

            // Skapa rotbokmärke
            PdfBookmarkEntry rootBookmark = new PdfBookmarkEntry
            {
                Text = "Root",
                Destination = sheet1.Cells["A1"],
                IsOpen = true
            };

            // Skapa underbokmärken
            PdfBookmarkEntry subBookmark1 = new PdfBookmarkEntry
            {
                Text = "Sheet2",
                Destination = sheet2.Cells["A1"]
            };

            PdfBookmarkEntry subBookmark2 = new PdfBookmarkEntry
            {
                Text = "Sheet3",
                Destination = sheet3.Cells["A1"]
            };

            // Lägg till underbokmärken till roten
            rootBookmark.SubEntry = new ArrayList { subBookmark1, subBookmark2 };

            // Konfigurera PDF-sparalternativ med bokmärken
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = rootBookmark
            };

            // Spara till minnesström (kan sparas till fil i verklig användning)
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Se även

* class [PdfBookmarkEntry](../../../aspose.cells.rendering/pdfbookmarkentry/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


