---
title: "Cell.Comment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el comentario de esta celda"
type: docs
url: /es/net/aspose.cells/cell/comment/
---
## Cell.Comment property

Obtiene el comentario de esta celda.

```csharp
public Comment Comment { get; }
```

### Observaciones

Si no hay ningún comentario aplicado a la celda, devuelve null.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyCommentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Cell");

            // Agregar un comentario a la celda
            Comment comment = cell.Comment;
            if (comment == null)
            {
                // Crear un nuevo comentario si no existe
                int commentIndex = worksheet.Comments.Add("A1");
                comment = worksheet.Comments[commentIndex];
                comment.Author = "Author Name";
                comment.Note = "This is a sample comment";
            }

            try
            {
                // Mostrar las propiedades del comentario
                Console.WriteLine("Comment Author: " + comment.Author);
                Console.WriteLine("Comment Note: " + comment.Note);
                Console.WriteLine("Comment Row: " + comment.Row);
                Console.WriteLine("Comment Column: " + comment.Column);
                Console.WriteLine("Comment is Visible: " + comment.IsVisible);

                // Modificar algunas propiedades del comentario
                comment.Note = "Updated comment text";
                comment.IsVisible = true;

                // Mostrar la nota del comentario actualizada
                Console.WriteLine("Updated Comment Note: " + comment.Note);

                // Guarda el libro de trabajo
                workbook.Save("CommentDemo.xlsx");
                Console.WriteLine("Comment has been demonstrated and saved to CommentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


