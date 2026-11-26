---
title: "PdfSaveOptions.PdfCompression"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Indica el algoritmo de compresión"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/pdfcompression/
---
## PdfSaveOptions.PdfCompression property

Indica el algoritmo de compresión

```csharp
public PdfCompressionCore PdfCompression { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyPdfCompressionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo y agregue datos de muestra
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample PDF Compression Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfCompression property usage");
            
            // Crear opciones de guardado PDF con compresión Flate
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PdfCompression = PdfCompressionCore.Flate;
            
            // Guardar el libro de trabajo como PDF con compresión
            workbook.Save("output_with_flate_compression.pdf", saveOptions);
            
            // Guardar nuevamente sin compresión para comparar
            saveOptions.PdfCompression = PdfCompressionCore.None;
            workbook.Save("output_without_compression.pdf", saveOptions);
            
            Console.WriteLine("PDF files created successfully with different compression settings.");
        }
    }
}
```

### Ver también

* enum [PdfCompressionCore](../../../aspose.cells.rendering/pdfcompressioncore/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


