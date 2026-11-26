---
title: "HtmlSaveOptions.IsExportComments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan los comentarios al guardar el archivo en HTML; el valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/isexportcomments/
---
## HtmlSaveOptions.IsExportComments property

Indica si se exportan los comentarios al guardar el archivo en HTML, el valor predeterminado es false.

```csharp
public bool IsExportComments { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsExportCommentsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo y comentarios
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Agregar un comentario
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";
            
            // Guardar con IsExportComments = false (los comentarios no se exportarán)
            HtmlSaveOptions options1 = new HtmlSaveOptions
            {
                IsExportComments = false
            };
            workbook.Save("output_without_comments.html", options1);
            
            // Guardar con IsExportComments = true (los comentarios se exportarán)
            HtmlSaveOptions options2 = new HtmlSaveOptions
            {
                IsExportComments = true
            };
            workbook.Save("output_with_comments.html", options2);
            
            Console.WriteLine("HTML files created successfully.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


