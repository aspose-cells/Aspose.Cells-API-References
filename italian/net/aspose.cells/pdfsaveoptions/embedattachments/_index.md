---
title: "PdfSaveOptions.EmbedAttachments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSaveOptions proprietà. Indica se incorporare l'allegato per gli oggetti Ole in Excel"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/embedattachments/
---
## PdfSaveOptions.EmbedAttachments property

Indica se incorporare gli allegati per gli oggetti Ole in Excel.

```csharp
public bool EmbedAttachments { get; set; }
```

### Osservazioni

Il valore predefinito è false. Il valore deve essere false quando la conformità PDF/A è impostata o la crittografia PDF è abilitata.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
using System.IO;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedAttachmentsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF with Embedded Attachments Example");

            // Crea un file di esempio da incorporare
            string sampleFile = "sample.docx";
            File.WriteAllText(sampleFile, "This is a sample document");

            // Aggiungi un allegato (oggetto OLE) al foglio di lavoro
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(sampleFile));
            worksheet.OleObjects[oleIndex].FileFormatType = FileFormatType.Docx;
            worksheet.OleObjects[oleIndex].DisplayAsIcon = true;

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Imposta la proprietà EmbedAttachments su true
            pdfSaveOptions.EmbedAttachments = true;

            // Salva la cartella di lavoro come PDF con allegati incorporati
            workbook.Save("PdfWithEmbeddedAttachments.pdf", pdfSaveOptions);

            // Pulisci
            File.Delete(sampleFile);
        }
    }
}
```

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


