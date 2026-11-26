---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor PdfSaveOptions. Crea las opciones para guardar un archivo PDF"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Crea las opciones para guardar un archivo pdf.

```csharp
public PdfSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Demostrar el constructor PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            
            // Guardar el libro de trabajo con opciones PDF
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("PDF saved successfully with PdfA1b compliance.");
        }
    }
}
```

### Ver también

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


