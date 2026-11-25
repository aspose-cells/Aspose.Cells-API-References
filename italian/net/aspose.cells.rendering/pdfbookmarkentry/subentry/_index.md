---
title: "PdfBookmarkEntry.SubEntry"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfBookmarkEntry. SubEntry di un segnalibro"
type: docs
url: /it/net/aspose.cells.rendering/pdfbookmarkentry/subentry/
---
## PdfBookmarkEntry.SubEntry property

SubEntry di un segnalibro.

```csharp
public ArrayList SubEntry { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Crea voce di segnalibro radice
            PdfBookmarkEntry root = new PdfBookmarkEntry
            {
                Text = "Main Bookmark",
                Destination = workbook.Worksheets[0].Cells["A1"],
                SubEntry = new ArrayList(),
                IsOpen = true
            };

            // Crea sotto-segnalibri
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

            // Aggiungi sotto-segnalibro annidato
            PdfBookmarkEntry subSub = new PdfBookmarkEntry
            {
                Text = "Sub-Section",
                Destination = workbook.Worksheets[2].Cells["B1"]
            };
            sub2.SubEntry.Add(subSub);

            // Aggiungi sotto-segnalibri alla radice
            root.SubEntry.Add(sub1);
            root.SubEntry.Add(sub2);

            // Salva con i segnalibri
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = root
            };
            workbook.Save("output_with_bookmarks.pdf", options);
        }
    }
}
```

### Vedi anche

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


