---
title: "PdfSaveOptions.EmbedAttachments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. Anger om bilagor för Ole-objekt i Excel ska bäddas in"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/embedattachments/
---
## PdfSaveOptions.EmbedAttachments property

Anger om bilagor för Ole‑objekt ska bäddas in i Excel.

```csharp
public bool EmbedAttachments { get; set; }
```

### Anmärkningar

Standardvärdet är falskt. Värdet måste vara falskt när PDF/A-efterlevnad är aktiverad eller pdf-kryptering är påslagen.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF with Embedded Attachments Example");

            // Skapa en exempelfil för inbäddning
            string sampleFile = "sample.docx";
            File.WriteAllText(sampleFile, "This is a sample document");

            // Lägg till en bilaga (OLE-objekt) i kalkylbladet
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(sampleFile));
            worksheet.OleObjects[oleIndex].FileFormatType = FileFormatType.Docx;
            worksheet.OleObjects[oleIndex].DisplayAsIcon = true;

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Ställ in EmbedAttachments-egenskapen till true
            pdfSaveOptions.EmbedAttachments = true;

            // Spara arbetsboken som PDF med inbäddade bilagor
            workbook.Save("PdfWithEmbeddedAttachments.pdf", pdfSaveOptions);

            // Rensa upp
            File.Delete(sampleFile);
        }
    }
}
```

### Se även

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


