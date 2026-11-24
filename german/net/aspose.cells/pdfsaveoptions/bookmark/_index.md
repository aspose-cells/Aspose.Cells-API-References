---
title: "PdfSaveOptions.Bookmark"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions-Eigenschaft. Gibt das PdfBookmarkEntry-Objekt zurück oder legt es fest."
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/bookmark/
---
## PdfSaveOptions.Bookmark property

Liest oder setzt das [`PdfBookmarkEntry`](../../../aspose.cells.rendering/pdfbookmarkentry/)-Objekt.

```csharp
public PdfBookmarkEntry Bookmark { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Füge drei Arbeitsblätter hinzu
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            Worksheet sheet3 = workbook.Worksheets.Add("Sheet3");

            // Setze Werte in Zellen, die als Lesezeichen-Ziele dienen.
            sheet1.Cells["A1"].Value = "Sheet1 Content";
            sheet2.Cells["A1"].Value = "Sheet2 Content";
            sheet3.Cells["A1"].Value = "Sheet3 Content";

            // Erstelle das Haupt-Lesezeichen.
            PdfBookmarkEntry rootBookmark = new PdfBookmarkEntry
            {
                Text = "Root",
                Destination = sheet1.Cells["A1"],
                IsOpen = true
            };

            // Erstelle Unter-Lesezeichen.
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

            // Füge Unter-Lesezeichen zum Haupt-Lesezeichen hinzu.
            rootBookmark.SubEntry = new ArrayList { subBookmark1, subBookmark2 };

            // Konfiguriere die PDF-Speicheroptionen mit Lesezeichen.
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = rootBookmark
            };

            // In Memory-Stream speichern (kann in realer Anwendung in eine Datei gespeichert werden).
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Siehe auch

* class [PdfBookmarkEntry](../../../aspose.cells.rendering/pdfbookmarkentry/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


