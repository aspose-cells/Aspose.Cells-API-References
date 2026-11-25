---
title: "PdfSaveOptions.DisplayDocTitle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSaveOptions proprietà. Indica se la barra del titolo di Windows deve visualizzare il titolo del documento"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/displaydoctitle/
---
## PdfSaveOptions.DisplayDocTitle property

Indica se la barra del titolo della finestra deve visualizzare il titolo del documento.

```csharp
public bool DisplayDocTitle { get; set; }
```

### Osservazioni

Se false, la barra del titolo dovrebbe invece visualizzare il nome del file PDF. Il valore predefinito è false.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF DisplayDocTitle Example");

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Imposta la proprietà DisplayDocTitle su true
            pdfSaveOptions.DisplayDocTitle = true;

            // Salva la cartella di lavoro come PDF
            workbook.Save("PdfDisplayDocTitleDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


