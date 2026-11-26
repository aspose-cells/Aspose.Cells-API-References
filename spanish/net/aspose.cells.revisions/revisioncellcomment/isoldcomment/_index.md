---
title: "RevisionCellComment.IsOldComment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellComment. Indica si es un comentario antiguo"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellcomment/isoldcomment/
---
## RevisionCellComment.IsOldComment property

Indica si es un comentario antiguo

```csharp
public bool IsOldComment { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyIsOldCommentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar comentario inicial a la celda A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "First version of comment";

            // Modificar el comentario para generar una revisión
            comment.Note = "Updated comment text";

            // Agregar otro comentario a la celda B2
            Comment secondComment = worksheet.Comments[1, 1];
            secondComment.Note = "Second comment";

            // Accede a las revisiones
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Mostrar el valor de la propiedad IsOldComment
                    Console.WriteLine("Cell: " + commentRevision.CellName);
                    Console.WriteLine("IsOldComment: " + commentRevision.IsOldComment);
                    
                    // Demostrar el uso de la propiedad IsOldComment
                    if (commentRevision.IsOldComment)
                    {
                        Console.WriteLine("This revision represents the old state of the comment");
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    }
                    else
                    {
                        Console.WriteLine("This revision represents the new state of the comment");
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }

                    // Mostrar propiedades relacionadas
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellCommentPropertyIsOldCommentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


