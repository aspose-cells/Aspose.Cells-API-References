---
title: "PdfSaveOptions.Compliance"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Obtiene o establece el nivel de cumplimiento de los estándares PDF para los documentos de salida"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Obtiene o establece el nivel de cumplimiento de normas PDF para los documentos de salida.

```csharp
public PdfCompliance Compliance { get; set; }
```

### Observaciones

El valor predeterminado es Pdf17.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyComplianceDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF Compliance");

            // Establecer las opciones de guardado PDF con cumplimiento PDF/A-1b
            PdfSaveOptions options = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b
            };

            // Guardar el libro de trabajo como PDF con configuraciones de cumplimiento
            workbook.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with PDF/A-1b compliance.");
        }
    }
}
```

### Ver también

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


