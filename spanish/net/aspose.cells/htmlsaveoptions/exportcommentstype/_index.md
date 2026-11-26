---
title: "HtmlSaveOptions.ExportCommentsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Representa el tipo de exportación de comentarios a archivos html"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportcommentstype/
---
## HtmlSaveOptions.ExportCommentsType property

Representa el tipo de exportación de comentarios a archivos html.

```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCommentsTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un comentario de ejemplo usando el nombre de la celda
            Comment comment = worksheet.Comments["A1"];
            comment.Note = "This is a test comment";
            
            // Establecer las opciones de guardado HTML con ExportCommentsType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
            
            // Guardar en HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file with comments exported successfully.");
        }
    }
}
```

### Ver también

* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


