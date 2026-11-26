---
title: "Comment.HtmlNote"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Obtiene y establece la cadena html que contiene datos y algunos formatos en este comentario"
type: docs
url: /es/net/aspose.cells/comment/htmlnote/
---
## Comment.HtmlNote property

Obtiene y establece la cadena html que contiene datos y algunos formatos en este comentario.

```csharp
public string HtmlNote { get; set; }
```

### Observaciones

Si este es un comentario en hilo, la nota no se puede cambiar, de lo contrario MS Excel no podría procesarlo como un comentario en hilo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHtmlNoteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            comment.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            
            workbook.Save("CommentHtmlNoteDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


