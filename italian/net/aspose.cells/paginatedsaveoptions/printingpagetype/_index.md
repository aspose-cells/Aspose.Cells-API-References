---
title: "PaginatedSaveOptions.PrintingPageType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Indica quali pagine non saranno stampate"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/printingpagetype/
---
## PaginatedSaveOptions.PrintingPageType property

Indica quali pagine non saranno stampate.

```csharp
public PrintingPageType PrintingPageType { get; set; }
```

### Osservazioni

Se il contenuto nel foglio è scarso, alcune pagine saranno totalmente vuote nel file PDF di output. Se non vuoi queste pagine vuote, puoi usare questa opzione per ometterle.

### Esempi

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
            
            // Aggiungi alcuni dati di esempio
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123);
            ws.Cells["A3"].PutValue(456);
            
            // Crea foglio di lavoro vuoto
            Worksheet blankWs = wb.Worksheets.Add("BlankSheet");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Salva ignorando le pagine vuote
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            wb.Save("output_ignore_blank_page.pdf", pdfSaveOptions);
            
            // Salva ignorando le pagine vuote e le pagine solo di stile
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;
            wb.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* enum [PrintingPageType](../../printingpagetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


