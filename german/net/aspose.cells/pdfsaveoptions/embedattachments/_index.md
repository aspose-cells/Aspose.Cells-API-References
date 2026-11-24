---
title: "PdfSaveOptions.EmbedAttachments"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions‑Eigenschaft. Gibt an, ob Anhänge für OLE‑Objekte in Excel eingebettet werden sollen"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/embedattachments/
---
## PdfSaveOptions.EmbedAttachments property

Gibt an, ob Anhänge für OLE-Objekte in Excel eingebettet werden sollen.

```csharp
public bool EmbedAttachments { get; set; }
```

### Hinweise

Der Standardwert ist false. Der Wert muss false sein, wenn PDF/A‑Konformität eingestellt ist oder PDF‑Verschlüsselung aktiviert ist.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF with Embedded Attachments Example");

            // Erstellen Sie eine Beispieldatei zum Einbetten
            string sampleFile = "sample.docx";
            File.WriteAllText(sampleFile, "This is a sample document");

            // Fügen Sie einen Anhang (OLE‑Objekt) zum Arbeitsblatt hinzu
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(sampleFile));
            worksheet.OleObjects[oleIndex].FileFormatType = FileFormatType.Docx;
            worksheet.OleObjects[oleIndex].DisplayAsIcon = true;

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Setzen Sie die EmbedAttachments‑Eigenschaft auf true
            pdfSaveOptions.EmbedAttachments = true;

            // Speichern Sie die Arbeitsmappe als PDF mit eingebetteten Anhängen
            workbook.Save("PdfWithEmbeddedAttachments.pdf", pdfSaveOptions);

            // Aufräumen
            File.Delete(sampleFile);
        }
    }
}
```

### Siehe auch

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


