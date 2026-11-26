---
title: "RevisionCellComment.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellComment. Obtiene el tipo de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellcomment/type/
---
## RevisionCellComment.Type property

Obtiene el tipo de revisión.

```csharp
public override RevisionType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentRow = 0;
            int commentCol = 0;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Seguimiento de revisiones - cambiado para usar la propiedad HasRevisions
            // Nota: En el uso real, puede que necesite habilitar el seguimiento por otros medios
            // ya que HasRevisions es una propiedad de solo lectura que indica si existen revisiones

            // Modificar el comentario para generar una revisión
            comment.Note = "Modified comment";

            // Acceda a las revisiones a través de la colección RevisionLogs del Workbook
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Mostrar el valor de la propiedad Type
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    
                    // Demostrar el uso de la propiedad Type
                    if (commentRevision.Type == RevisionType.Comment)
                    {
                        Console.WriteLine("This revision is related to a comment change");
                        Console.WriteLine("Comment was modified at row: " + commentRevision.Row + ", column: " + commentRevision.Column);
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellCommentPropertyTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


