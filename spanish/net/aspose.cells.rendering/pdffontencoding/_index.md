---
title: "Enum PdfFontEncoding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Rendering.PdfFontEncoding. Representa la codificación de fuentes incrustadas en PDF"
type: docs
url: /es/net/aspose.cells.rendering/pdffontencoding/
---
## PdfFontEncoding enumeration

Representa la codificación de fuentes incrustadas PDF.

```csharp
public enum PdfFontEncoding
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Identity | `0` | Representa el uso de la codificación Identity-H para todas las fuentes incrustadas en PDF. |
| AnsiPrefer | `1` | Representa la preferencia de usar WinAnsiEncoding para fuentes TrueType con caracteres 32-127; de lo contrario, se usará la codificación Identity-H para las fuentes incrustadas en PDF. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfFontEncodingDemo
    {
        public static void PdfFontEncodingExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");

            // Crea PdfSaveOptions y establece la propiedad FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;

            // Guarda el libro de trabajo como un archivo PDF
            workbook.Save("PdfFontEncodingExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file created successfully with specified font encoding.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


