---
title: "Klasse PdfBookmarkEntry"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.PdfBookmarkEntry Klasse. PdfBookmarkEntry ist ein Eintrag im PDF-Lesezeichen. Wenn die Text‑Eigenschaft der aktuellen Instanz null ist, wird die aktuelle Instanz ausgeblendet und die Kind‑Einträge werden auf derselben Ebene eingefügt."
type: docs
url: /de/net/aspose.cells.rendering/pdfbookmarkentry/
---
## PdfBookmarkEntry class

PdfBookmarkEntry ist ein Eintrag im PDF-Lesezeichen. Wenn die Text‑Eigenschaft der aktuellen Instanz null oder \"\" ist, wird die aktuelle Instanz ausgeblendet und die Kinder werden auf derselben Ebene eingefügt.

```csharp
public class PdfBookmarkEntry
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PdfBookmarkEntry](pdfbookmarkentry/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Destination](../../aspose.cells.rendering/pdfbookmarkentry/destination/) { get; set; } | Die Zelle, zu der der Lesezeichen‑Link führt. |
| [DestinationName](../../aspose.cells.rendering/pdfbookmarkentry/destinationname/) { get; set; } | Liest oder setzt den Namen des Ziels. |
| [IsCollapse](../../aspose.cells.rendering/pdfbookmarkentry/iscollapse/) { get; set; } | Wenn diese Eigenschaft true ist, wird das bookmarkentry zusammengeklappt, andernfalls wird es erweitert. |
| [IsOpen](../../aspose.cells.rendering/pdfbookmarkentry/isopen/) { get; set; } | Wenn diese Eigenschaft true ist, wird das bookmarkentry erweitert, andernfalls wird es zusammengeklappt. |
| [SubEntry](../../aspose.cells.rendering/pdfbookmarkentry/subentry/) { get; set; } | Unter­eintrag eines Lesezeichens. |
| [Text](../../aspose.cells.rendering/pdfbookmarkentry/text/) { get; set; } | Titel eines Lesezeichens. |

### Beispiele

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
            // Neue Arbeitsmappe erstellen und Arbeitsblätter hinzufügen
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Zellen aus jedem Arbeitsblatt abrufen
            Cell cellInPage1 = workbook.Worksheets[0].Cells["A1"];
            Cell cellInPage2 = workbook.Worksheets[1].Cells["A1"];
            Cell cellInPage3 = workbook.Worksheets[2].Cells["A1"];

            // Werte in die Zellen einfügen
            cellInPage1.PutValue("page1");
            cellInPage2.PutValue("page2");
            cellInPage3.PutValue("page3");

            // Root‑PdfBookmarkEntry erstellen
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry
            {
                Text = "root",  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
                Destination = cellInPage1,
                SubEntry = new ArrayList(),
                IsOpen = false
            };

            // Unter‑PdfBookmarkEntries erstellen
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

            // Unter­einträge zum Root‑Eintrag hinzufügen
            pbeRoot.SubEntry.Add(subPbe1);
            pbeRoot.SubEntry.Add(subPbe2);

            // PdfSaveOptions erstellen und das Lesezeichen setzen
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Bookmark = pbeRoot
            };

            // Speichern Sie die Arbeitsmappe als PDF mit Lesezeichen
            workbook.Save("output_bookmark.pdf", saveOptions);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


