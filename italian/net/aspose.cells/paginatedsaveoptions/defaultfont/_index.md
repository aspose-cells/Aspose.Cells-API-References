---
title: "PaginatedSaveOptions.DefaultFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Quando i caratteri in Excel sono Unicode e non vengono impostati con il font corretto nello stile della cella, possono apparire come blocchi nell'immagine PDF. Imposta DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per mostrare questi caratteri Unicode"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/defaultfont/
---
## PaginatedSaveOptions.DefaultFont property

Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per mostrare questi caratteri Unicode.

```csharp
public string DefaultFont { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("This text will use the default font");
            worksheet.Cells["A2"].PutValue("如果默认字体支持中文，这将显示正确");

            // Configura le opzioni di salvataggio PDF con il font predefinito
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultFont = "宋体";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;

            // Salva in PDF
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


