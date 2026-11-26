---
title: "PaginatedSaveOptions.CheckWorkbookDefaultFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Cuando los caracteres en el Excel son Unicode y no se establecen con la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdfimage. Establezca esto en true para intentar usar la fuente predeterminada del libro de trabajo para mostrar estos caracteres primero."
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/
---
## PaginatedSaveOptions.CheckWorkbookDefaultFont property

Cuando los caracteres en el Excel son Unicode y no se establece una fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo y mostrar estos caracteres primero.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Test Content");
            
            // Configurar opciones de guardado de PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CheckWorkbookDefaultFont = false;
            
            // Guardar como PDF
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF saved with CheckWorkbookDefaultFont set to false");
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


