---
title: "Enum PdfCompressionCore"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Rendering.PdfCompressionCore. Especifica un tipo de compresión aplicado a todo el contenido del archivo PDF, excepto a las imágenes"
type: docs
url: /es/net/aspose.cells.rendering/pdfcompressioncore/
---
## PdfCompressionCore enumeration

Especifica un tipo de compresión aplicado a todo el contenido del archivo PDF, excepto a las imágenes.

```csharp
public enum PdfCompressionCore
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Ninguno |
| Rle | `1` | Rle |
| Lzw | `2` | Lzw |
| Flate | `3` | Flate |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfCompressionCoreDemo
    {
        public static void PdfCompressionCoreExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose!");

            // Crear PdfSaveOptions y establecer el PdfCompressionCore
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate; // Setting the compression type to Flate

            // Guardar el libro de trabajo como un archivo PDF con la compresión especificada
            workbook.Save("PdfCompressionCoreExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file saved with specified compression.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


