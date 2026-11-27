---
title: "Klass PdfBookmarkEntry"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.PdfBookmarkEntry klass. PdfBookmarkEntry är ett objekt i pdf‑bokmärket. om Text‑egenskapen för den aktuella instansen är null eller den aktuella instansen kommer att döljas och barn kommer att infogas på samma nivå"
type: docs
url: /sv/net/aspose.cells.rendering/pdfbookmarkentry/
---
## PdfBookmarkEntry class

PdfBookmarkEntry är ett objekt i pdf-bokmärken. Om Text‑egenskapen för den aktuella instansen är null eller "", kommer den aktuella instansen att döljas och barnen kommer att infogas på samma nivå.

```csharp
public class PdfBookmarkEntry
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PdfBookmarkEntry](pdfbookmarkentry/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Destination](../../aspose.cells.rendering/pdfbookmarkentry/destination/) { get; set; } | Cellen som bokmärkeslänken pekar på. |
| [DestinationName](../../aspose.cells.rendering/pdfbookmarkentry/destinationname/) { get; set; } | Hämtar eller anger namn på destinationen. |
| [IsCollapse](../../aspose.cells.rendering/pdfbookmarkentry/iscollapse/) { get; set; } | När denna egenskap är sann kommer bookmarkentry att kollapsa, annars expanderar den. |
| [IsOpen](../../aspose.cells.rendering/pdfbookmarkentry/isopen/) { get; set; } | När denna egenskap är sann kommer bookmarkentry att expandera, annars kollapsar den. |
| [SubEntry](../../aspose.cells.rendering/pdfbookmarkentry/subentry/) { get; set; } | Underpost för ett bokmärke. |
| [Text](../../aspose.cells.rendering/pdfbookmarkentry/text/) { get; set; } | Titel för ett bokmärke. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Collections;

    public class PdfBookmarkEntryDemo
    {
        public static void PdfBookmarkEntryExample()
        {
            // Skapa en ny arbetsbok och lägg till kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Hämta celler från varje kalkylblad
            Cell cellInPage1 = workbook.Worksheets[0].Cells["A1"];
            Cell cellInPage2 = workbook.Worksheets[1].Cells["A1"];
            Cell cellInPage3 = workbook.Worksheets[2].Cells["A1"];

            // Sätt värden i cellerna
            cellInPage1.PutValue("page1");
            cellInPage2.PutValue("page2");
            cellInPage3.PutValue("page3");

            // Skapa rot‑PdfBookmarkEntry
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry
            {
                Text = "root",  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
                Destination = cellInPage1,
                SubEntry = new ArrayList(),
                IsOpen = false
            };

            // Skapa under‑PdfBookmarkEntries
            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry
            {
                Text = "section1",
                Destination = cellInPage2
            };

            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry
            {
                Text = "section2",
                Destination = cellInPage3
            };

            // Lägg till underposter i rotposten
            pbeRoot.SubEntry.Add(subPbe1);
            pbeRoot.SubEntry.Add(subPbe2);

            // Skapa PdfSaveOptions och ange bokmärket
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Bookmark = pbeRoot
            };

            // Spara arbetsboken som en PDF med bokmärken
            workbook.Save("output_bookmark.pdf", saveOptions);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


