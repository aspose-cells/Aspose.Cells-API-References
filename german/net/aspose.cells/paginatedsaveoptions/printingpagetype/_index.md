---
title: "PaginatedSaveOptions.PrintingPageType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt an, welche Seiten nicht gedruckt werden"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/printingpagetype/
---
## PaginatedSaveOptions.PrintingPageType property

Gibt an, welche Seiten nicht gedruckt werden.

```csharp
public PrintingPageType PrintingPageType { get; set; }
```

### Hinweise

Wenn der Inhalt im Blatt spärlich ist, können einige Seiten im ausgegebenen PDF völlig leer sein. Wenn Sie diese leeren Seiten nicht möchten, können Sie diese Option verwenden, um sie zu entfernen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPrintingPageTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Fügen Sie einige Beispieldaten hinzu
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123);
            ws.Cells["A3"].PutValue(456);
            
            // Leeres Arbeitsblatt erstellen
            Worksheet blankWs = wb.Worksheets.Add("BlankSheet");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Speichern, leere Seiten ignorieren
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            wb.Save("output_ignore_blank_page.pdf", pdfSaveOptions);
            
            // Speichern, leere Seiten und rein stilistische Seiten ignorieren
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;
            wb.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* enum [PrintingPageType](../../printingpagetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


