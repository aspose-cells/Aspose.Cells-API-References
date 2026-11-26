---
title: "PaginatedSaveOptions.PrintingPageType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Indica qué páginas no se imprimirán"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/printingpagetype/
---
## PaginatedSaveOptions.PrintingPageType property

Indica qué páginas no se imprimirán.

```csharp
public PrintingPageType PrintingPageType { get; set; }
```

### Observaciones

Si el contenido en la hoja es escaso, habrá algunas páginas totalmente en blanco en el archivo PDF de salida. Si no deseas esas páginas en blanco, puedes usar esta opción para omitirlas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPrintingPageTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Agregar algunos datos de ejemplo
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123);
            ws.Cells["A3"].PutValue(456);
            
            // Crear hoja de cálculo en blanco
            Worksheet blankWs = wb.Worksheets.Add("BlankSheet");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Guardar ignorando páginas en blanco
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            wb.Save("output_ignore_blank_page.pdf", pdfSaveOptions);
            
            // Guardar ignorando páginas en blanco y páginas solo de estilo
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;
            wb.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* enum [PrintingPageType](../../printingpagetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


