---
title: "PdfSaveOptions.DisplayDocTitle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Indica si la barra de título de Windows debe mostrar el título del documento"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/displaydoctitle/
---
## PdfSaveOptions.DisplayDocTitle property

Indica si la barra de título de la ventana debe mostrar el título del documento.

```csharp
public bool DisplayDocTitle { get; set; }
```

### Observaciones

Si es false, la barra de título debe mostrar en su lugar el nombre del archivo PDF. El valor predeterminado es false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyDisplayDocTitleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF DisplayDocTitle Example");

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Establecer la propiedad DisplayDocTitle a true
            pdfSaveOptions.DisplayDocTitle = true;

            // Guardar el libro de trabajo como PDF
            workbook.Save("PdfDisplayDocTitleDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


