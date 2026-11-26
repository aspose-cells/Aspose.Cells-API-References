---
title: "HtmlSaveOptions.DisableDownlevelRevealedComments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "HtmlSaveOptions propiedad. Indica si se deshabilitan los comentarios condicionales Downlevelrevealed al exportar el archivo a html; el valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/
---
## HtmlSaveOptions.DisableDownlevelRevealedComments property

Indica si se deshabilitan los comentarios condicionales revelados de nivel inferior al exportar el archivo a html, el valor predeterminado es false.

```csharp
public bool DisableDownlevelRevealedComments { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDisableDownlevelRevealedCommentsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con un comentario
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a test comment";

            // Establecer opciones de guardado HTML con DisableDownlevelRevealedComments
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DisableDownlevelRevealedComments = true;

            // Guardar el libro de trabajo con opciones HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("Workbook saved with DisableDownlevelRevealedComments=true");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


