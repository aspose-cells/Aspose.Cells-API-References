---
title: "PdfSaveOptions.DisplayDocTitle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions‑Eigenschaft. Gibt an, ob die Titelleiste von Windows den Dokumenttitel anzeigen soll"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/displaydoctitle/
---
## PdfSaveOptions.DisplayDocTitle property

Gibt an, ob die Titelleiste des Fensters den Dokumenttitel anzeigen soll.

```csharp
public bool DisplayDocTitle { get; set; }
```

### Hinweise

Wenn false, sollte die Titelleiste stattdessen den Namen der PDF‑Datei anzeigen. Der Standardwert ist false.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyDisplayDocTitleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF DisplayDocTitle Example");

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Setzen Sie die DisplayDocTitle‑Eigenschaft auf true
            pdfSaveOptions.DisplayDocTitle = true;

            // Speichern Sie die Arbeitsmappe als PDF
            workbook.Save("PdfDisplayDocTitleDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


