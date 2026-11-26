---
title: "PdfSaveOptions.EmbedAttachments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Indica si se debe incrustar el adjunto para objetos OLE en Excel"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/embedattachments/
---
## PdfSaveOptions.EmbedAttachments property

Indica si se debe incrustar el adjunto para objetos Ole en Excel.

```csharp
public bool EmbedAttachments { get; set; }
```

### Observaciones

El valor predeterminado es false. El valor debe ser false cuando se establece la conformidad PDF/A o el cifrado PDF está habilitado.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF with Embedded Attachments Example");

            // Crear un archivo de muestra para incrustar
            string sampleFile = "sample.docx";
            File.WriteAllText(sampleFile, "This is a sample document");

            // Agregar un adjunto (objeto OLE) a la hoja de cálculo
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(sampleFile));
            worksheet.OleObjects[oleIndex].FileFormatType = FileFormatType.Docx;
            worksheet.OleObjects[oleIndex].DisplayAsIcon = true;

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Establecer la propiedad EmbedAttachments a true
            pdfSaveOptions.EmbedAttachments = true;

            // Guardar el libro de trabajo como PDF con adjuntos incrustados
            workbook.Save("PdfWithEmbeddedAttachments.pdf", pdfSaveOptions);

            // Limpiar
            File.Delete(sampleFile);
        }
    }
}
```

### Ver también

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


