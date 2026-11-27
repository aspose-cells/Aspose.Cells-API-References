---
title: "PdfBookmarkEntry.SubEntry"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfBookmarkEntry-egenskap. Underpost för ett bokmärke"
type: docs
url: /sv/net/aspose.cells.rendering/pdfbookmarkentry/subentry/
---
## PdfBookmarkEntry.SubEntry property

Underpost för ett bokmärke.

```csharp
public ArrayList SubEntry { get; set; }
```

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertySubEntryDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Skapa rotbokmärkespost
            PdfBookmarkEntry root = new PdfBookmarkEntry
            {
                Text = "Main Bookmark",
                Destination = workbook.Worksheets[0].Cells["A1"],
                SubEntry = new ArrayList(),
                IsOpen = true
            };

            // Skapa underbokmärken
            PdfBookmarkEntry sub1 = new PdfBookmarkEntry
            {
                Text = "First Section",
                Destination = workbook.Worksheets[1].Cells["A1"]
            };

            PdfBookmarkEntry sub2 = new PdfBookmarkEntry
            {
                Text = "Second Section",
                Destination = workbook.Worksheets[2].Cells["A1"],
                SubEntry = new ArrayList()
            };

            // Lägg till nästlad underbokmärke
            PdfBookmarkEntry subSub = new PdfBookmarkEntry
            {
                Text = "Sub-Section",
                Destination = workbook.Worksheets[2].Cells["B1"]
            };
            sub2.SubEntry.Add(subSub);

            // Lägg till underbokmärken till roten
            root.SubEntry.Add(sub1);
            root.SubEntry.Add(sub2);

            // Spara med bokmärken
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = root
            };
            workbook.Save("output_with_bookmarks.pdf", options);
        }
    }
}
```

### Se även

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


