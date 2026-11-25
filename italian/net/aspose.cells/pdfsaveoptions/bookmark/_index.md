---
title: "PdfSaveOptions.Bookmark"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSaveOptions. Ottiene e imposta l'oggetto PdfBookmarkEntry"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/bookmark/
---
## PdfSaveOptions.Bookmark property

Ottiene e imposta l'oggetto [`PdfBookmarkEntry`](../../../aspose.cells.rendering/pdfbookmarkentry/).

```csharp
public PdfBookmarkEntry Bookmark { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi tre fogli di lavoro
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            Worksheet sheet3 = workbook.Worksheets.Add("Sheet3");

            // Imposta i valori nelle celle che saranno destinazioni dei segnalibri
            sheet1.Cells["A1"].Value = "Sheet1 Content";
            sheet2.Cells["A1"].Value = "Sheet2 Content";
            sheet3.Cells["A1"].Value = "Sheet3 Content";

            // Crea segnalibro radice
            PdfBookmarkEntry rootBookmark = new PdfBookmarkEntry
            {
                Text = "Root",
                Destination = sheet1.Cells["A1"],
                IsOpen = true
            };

            // Crea sotto-segnalibri
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

            // Aggiungi sotto-segnalibri alla radice
            rootBookmark.SubEntry = new ArrayList { subBookmark1, subBookmark2 };

            // Configura le opzioni di salvataggio PDF con i segnalibri
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = rootBookmark
            };

            // Salva su stream di memoria (potrebbe salvare su file in un utilizzo reale)
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Vedi anche

* class [PdfBookmarkEntry](../../../aspose.cells.rendering/pdfbookmarkentry/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


