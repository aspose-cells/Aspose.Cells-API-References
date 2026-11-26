---
title: "RevisionCellComment.NewLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellComment. Obtiene la longitud del comentario antes de que se hiciera esta revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellcomment/newlength/
---
## RevisionCellComment.NewLength property

Obtiene la longitud del comentario antes de que se hiciera esta revisión

```csharp
public int NewLength { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyNewLengthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda F7
            int commentRow = 6;
            int commentCol = 5;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment text";

            // Modificar el comentario para generar una revisión
            string updatedComment = "This is an updated and longer comment text";
            comment.Note = updatedComment;

            // Accede a las revisiones
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Mostrar el valor de la propiedad NewLength
                    Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    Console.WriteLine("Actual new comment length: " + updatedComment.Length);
                    
                    // Muestra propiedades relacionadas
                    Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    
                    // Demostrar el uso de la propiedad NewLength
                    if (commentRevision.NewLength > commentRevision.OldLength)
                    {
                        Console.WriteLine("Comment was expanded by " + 
                            (commentRevision.NewLength - commentRevision.OldLength) + " characters");
                    }
                    else if (commentRevision.NewLength < commentRevision.OldLength)
                    {
                        Console.WriteLine("Comment was shortened by " + 
                            (commentRevision.OldLength - commentRevision.NewLength) + " characters");
                    }
                    else
                    {
                        Console.WriteLine("Comment length remained the same");
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellCommentPropertyNewLengthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


