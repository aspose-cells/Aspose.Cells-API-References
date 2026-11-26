---
title: "Clase RevisionCellComment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionCellComment. Representa un registro de revisión de un cambio en el comentario de una celda"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellcomment/
---
## RevisionCellComment class

Representa un registro de revisión de un cambio en el comentario de una celda.

```csharp
public class RevisionCellComment : Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncellcomment/actiontype/) { get; } | Obtiene el tipo de acción de la revisión. |
| [CellName](../../aspose.cells.revisions/revisioncellcomment/cellname/) { get; set; } | Obtiene el nombre de la celda. |
| [Column](../../aspose.cells.revisions/revisioncellcomment/column/) { get; } | Obtiene el índice de columna que contiene un comentario |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión.(Heredado de [`Revision`](../revision/).) |
| [IsOldComment](../../aspose.cells.revisions/revisioncellcomment/isoldcomment/) { get; } | Indica si es un comentario antiguo |
| [NewLength](../../aspose.cells.revisions/revisioncellcomment/newlength/) { get; } | Obtiene la longitud del comentario antes de que se hiciera esta revisión |
| [OldLength](../../aspose.cells.revisions/revisioncellcomment/oldlength/) { get; } | Obtiene la longitud del texto del comentario añadido en esta revisión |
| [Row](../../aspose.cells.revisions/revisioncellcomment/row/) { get; } | Obtiene el índice de fila que contiene un comentario |
| override [Type](../../aspose.cells.revisions/revisioncellcomment/type/) { get; } | Obtiene el tipo de revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. (Heradado de [`Revision`](../revision/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCellCommentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar comentario inicial a la celda A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment text";

            // Modificar el comentario para generar una revisión
            comment.Note = "Updated comment with more text";

            // Acceder al registro de revisiones
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;

                    // Mostrar propiedades de la revisión
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("Row: " + commentRevision.Row);
                    Console.WriteLine("Column: " + commentRevision.Column);

                    // Mostrar cambios en la longitud del comentario
                    Console.WriteLine("Old Length: " + commentRevision.OldLength);
                    Console.WriteLine("New Length: " + commentRevision.NewLength);
                    Console.WriteLine("Is Old Comment: " + commentRevision.IsOldComment);

                    // Modificar el nombre de la celda para demostrar el cambio de propiedad
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "B2";
                    Console.WriteLine("Modified Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("New Row: " + commentRevision.Row);
                    Console.WriteLine("New Column: " + commentRevision.Column);

                    // Restaurar el nombre original de la celda
                    commentRevision.CellName = originalCellName;
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionsClassRevisionCellCommentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


