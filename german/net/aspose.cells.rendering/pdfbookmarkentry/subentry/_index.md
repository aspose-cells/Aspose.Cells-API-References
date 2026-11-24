---
title: "PdfBookmarkEntry.SubEntry"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfBookmarkEntry-Eigenschaft. Untereintrag eines Lesezeichens"
type: docs
url: /de/net/aspose.cells.rendering/pdfbookmarkentry/subentry/
---
## PdfBookmarkEntry.SubEntry property

Unter­eintrag eines Lesezeichens.

```csharp
public ArrayList SubEntry { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Root-Lesezeicheneintrag erstellen
            PdfBookmarkEntry root = new PdfBookmarkEntry
            {
                Text = "Main Bookmark",
                Destination = workbook.Worksheets[0].Cells["A1"],
                SubEntry = new ArrayList(),
                IsOpen = true
            };

            // Erstelle Unter-Lesezeichen.
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

            // Verschachtelten Unter-Lesezeichen hinzufügen
            PdfBookmarkEntry subSub = new PdfBookmarkEntry
            {
                Text = "Sub-Section",
                Destination = workbook.Worksheets[2].Cells["B1"]
            };
            sub2.SubEntry.Add(subSub);

            // Füge Unter-Lesezeichen zum Haupt-Lesezeichen hinzu.
            root.SubEntry.Add(sub1);
            root.SubEntry.Add(sub2);

            // Mit Lesezeichen speichern
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = root
            };
            workbook.Save("output_with_bookmarks.pdf", options);
        }
    }
}
```

### Siehe auch

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


