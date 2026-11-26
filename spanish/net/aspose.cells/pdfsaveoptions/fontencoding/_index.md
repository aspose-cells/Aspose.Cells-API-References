---
title: "PdfSaveOptions.FontEncoding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Obtiene o establece la codificación de fuente incrustada en el pdf"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/fontencoding/
---
## PdfSaveOptions.FontEncoding property

Obtiene o establece la codificación de fuentes incrustadas en pdf.

```csharp
public PdfFontEncoding FontEncoding { get; set; }
```

### Observaciones

El valor predeterminado es Identity

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyFontEncodingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Font Encoding Test");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfFontEncoding usage");

            // Configurar opciones de guardado PDF con FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.DefaultFont = "Arial";

            // Guarda el libro de trabajo en PDF
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* enum [PdfFontEncoding](../../../aspose.cells.rendering/pdffontencoding/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


