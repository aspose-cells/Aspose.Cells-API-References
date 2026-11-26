---
title: "RevisionCellComment.ActionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellComment. Obtiene el tipo de acción de la revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellcomment/actiontype/
---
## RevisionCellComment.ActionType property

Obtiene el tipo de acción de la revisión.

```csharp
public RevisionActionType ActionType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment";

            // Modificar el comentario para generar una revisión
            comment.Note = "Updated comment";

            // Agregue un nuevo comentario para generar una revisión Add
            Comment newComment = worksheet.Comments[1, 1];
            newComment.Note = "New comment";

            // Accede a las revisiones
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Muestre el valor de la propiedad ActionType
                    Console.WriteLine("Revision ActionType: " + commentRevision.ActionType);
                    
                    // Demostrar el uso de la propiedad ActionType
                    switch (commentRevision.ActionType)
                    {
                        case RevisionActionType.Add:
                            Console.WriteLine("This revision added a new comment at " + commentRevision.CellName);
                            break;
                        case RevisionActionType.Delete:
                            Console.WriteLine("This revision deleted a comment from " + commentRevision.CellName);
                            break;
                        default:
                            Console.WriteLine("This revision modified a comment at " + commentRevision.CellName);
                            break;
                    }

                    // Mostrar propiedades relacionadas
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    Console.WriteLine("Is old comment: " + commentRevision.IsOldComment);
                    Console.WriteLine("Old length: " + commentRevision.OldLength);
                    Console.WriteLine("New length: " + commentRevision.NewLength);
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellCommentPropertyActionTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


