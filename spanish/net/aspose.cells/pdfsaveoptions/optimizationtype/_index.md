---
title: "PdfSaveOptions.OptimizationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Obtiene y establece el tipo de optimización pdf"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/optimizationtype/
---
## PdfSaveOptions.OptimizationType property

Obtiene y establece el tipo de optimización pdf.

```csharp
public PdfOptimizationType OptimizationType { get; set; }
```

### Observaciones

El valor predeterminado es Standard

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyOptimizationTypeDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Optimization Example");

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Demostrar la propiedad OptimizationType
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Guardar el libro de trabajo con configuraciones de optimización
            workbook.Save("OptimizedPdf.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* enum [PdfOptimizationType](../../../aspose.cells.rendering/pdfoptimizationtype/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


