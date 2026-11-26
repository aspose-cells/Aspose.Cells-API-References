---
title: "Clase Comment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Comment. Encapsula el objeto que representa un comentario de celda"
type: docs
url: /es/net/aspose.cells/comment/
---
## Comment class

Encapsula el objeto que representa un comentario de celda.

```csharp
public class Comment
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Author](../../aspose.cells/comment/author/) { get; set; } | Obtiene y establece el Nombre del autor original del comentario |
| [AutoSize](../../aspose.cells/comment/autosize/) { get; set; } | Indica si el tamaño del comentario se ajusta automáticamente según su contenido. Nota: En algunos casos especiales (como el entorno Mac), esta configuración puede no tener efecto. Si esta configuración no tiene efecto, por favor reemplácela con FitToTextSize(). |
| [Column](../../aspose.cells/comment/column/) { get; } | Obtiene el índice de columna del comentario. |
| [CommentShape](../../aspose.cells/comment/commentshape/) { get; } | Obtén un objeto Shape que representa la forma adjunta al comentario especificado. |
| [Font](../../aspose.cells/comment/font/) { get; } | Obtiene la fuente del comentario. |
| [Height](../../aspose.cells/comment/height/) { get; set; } | Representa la altura del comentario, en unidades de píxeles. |
| [HeightCM](../../aspose.cells/comment/heightcm/) { get; set; } | Representa la altura del comentario, en unidades de centímetros. |
| [HeightInch](../../aspose.cells/comment/heightinch/) { get; set; } | Representa la altura del comentario, en unidades de pulgadas. |
| [HtmlNote](../../aspose.cells/comment/htmlnote/) { get; set; } | Obtiene y establece la cadena html que contiene datos y algunos formatos en este comentario. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment/) { get; } | Indica si este comentario es un comentario en hilo. |
| [IsVisible](../../aspose.cells/comment/isvisible/) { get; set; } | Representa si el comentario es visible o no. |
| [Note](../../aspose.cells/comment/note/) { get; set; } | Representa el contenido del comentario. |
| [Row](../../aspose.cells/comment/row/) { get; } | Obtiene el índice de fila del comentario. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment/) { get; set; } | Obtiene y establece el tipo de alineación horizontal del texto del comentario. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype/) { get; set; } | Obtiene y establece el tipo de orientación del texto del comentario. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment/) { get; set; } | Obtiene y establece el tipo de alineación vertical del texto del comentario. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments/) { get; } | Obtiene la lista de comentarios en hilo; |
| [Width](../../aspose.cells/comment/width/) { get; set; } | Representa el ancho del comentario, en unidades de píxeles. |
| [WidthCM](../../aspose.cells/comment/widthcm/) { get; set; } | Representa el ancho del comentario, en unidades de centímetros. |
| [WidthInch](../../aspose.cells/comment/widthinch/) { get; set; } | Representa el ancho del comentario, en unidades de pulgadas. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters/)(int, int) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto del comentario. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters/)(int, int, Font, StyleFlag) | Formatea algunos caracteres con la configuración de fuente. |
| [GetRichFormattings](../../aspose.cells/comment/getrichformattings/)() | Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto del comentario. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CommentDemo
    {
        public static void CommentExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            // Accede a la colección de comentarios de la hoja de cálculo
            CommentCollection comments = worksheet.Comments;

            // Agregar un comentario a la celda A1
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Font.Name = "Times New Roman";
            comment1.Font.Size = 12;
            comment1.Font.Color = System.Drawing.Color.Red;
            comment1.Author = "Carl.Yang";
            comment1.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            comment1.IsVisible = true;
            comment1.TextOrientationType = TextOrientationType.TopToBottom;
            comment1.TextHorizontalAlignment = TextAlignmentType.Center;
            comment1.TextVerticalAlignment = TextAlignmentType.Center;
            comment1.AutoSize = true;
            comment1.HeightCM = 1.0;
            comment1.WidthCM = 1.0;
            comment1.Width = 10;
            comment1.Height = 10;
            comment1.WidthInch = 1.0;
            comment1.HeightInch = 1.0;

            // Accede a la forma del comentario
            CommentShape shape = comment1.CommentShape;
            int w = shape.Width;
            int h = shape.Height;

            // Agregar un comentario a la celda B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";

            // Guarda el libro de trabajo
            workbook.Save("CommentExample.xlsx");
            workbook.Save("CommentExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


