---
title: "Clase PdfConverter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.PdfConverter. Convertidor para convertir el archivo de plantilla a pdf"
type: docs
url: /es/net/aspose.cells.lowcode/pdfconverter/
---
## PdfConverter class

Convertidor para convertir archivos de plantilla a pdf.

```csharp
public class PdfConverter
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Convierte el archivo de plantilla a pdf |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process_1)(string, string) | Convierte el archivo de plantilla dado a pdf. |

### Ejemplos

```csharp
using System;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassPdfConverterDemo
    {
        public static void Run()
        {
            // Inicializa el PdfConverter con las rutas de plantilla y salida
            PdfConverter.Process("template.xlsx", "res.pdf");
            
            Console.WriteLine("PDF conversion completed successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


