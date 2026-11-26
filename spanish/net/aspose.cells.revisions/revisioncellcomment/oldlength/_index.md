---
title: "RevisionCellComment.OldLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellComment. Obtiene la longitud del texto del comentario añadido en esta revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellcomment/oldlength/
---
## RevisionCellComment.OldLength property

Obtiene la longitud del texto del comentario añadido en esta revisión

```csharp
public int OldLength { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyOldLengthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade un comentario a la celda D4
            int commentRow = 3;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            string initialComment = "Original comment text";
            comment.Note = initialComment;

            // Modificar el comentario para generar una revisión
            string updatedComment = "This is the modified comment text with more content";
            comment.Note = updatedComment;

            // Accede a las revisiones
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Muestra el valor de la propiedad OldLength
                    Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    Console.WriteLine("Actual initial comment length: " + initialComment.Length);
                    
                    // Muestra propiedades relacionadas
                    Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    
                    // Demuestra el uso de la propiedad OldLength
                    if (commentRevision.OldLength > 0)
                    {
                        Console.WriteLine("Comment existed before modification with length: " + 
                            commentRevision.OldLength);
                            
                        double expansionPercentage = ((double)(commentRevision.NewLength - commentRevision.OldLength) / 
                            commentRevision.OldLength) * 100;
                        Console.WriteLine($"Comment expanded by {expansionPercentage:F2}%");
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellCommentPropertyOldLengthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


