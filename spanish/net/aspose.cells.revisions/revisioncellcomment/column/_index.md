---
title: "RevisionCellComment.Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellComment. Obtiene el índice de columna que contiene un comentario"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellcomment/column/
---
## RevisionCellComment.Column property

Obtiene el índice de columna que contiene un comentario

```csharp
public int Column { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda D3
            int commentRow = 2;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Sample comment for revision tracking";

            // Modificar el comentario para generar una revisión
            comment.Note = "Updated comment text";

            // Accede a las revisiones
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Mostrar el valor de la propiedad Column
                    Console.WriteLine("Comment revision column index: " + commentRevision.Column);
                    
                    // Demostrar el uso de la propiedad Column
                    Console.WriteLine("Comment was modified in column: " + (char)('A' + commentRevision.Column));
                    
                    // Mostrar propiedades relacionadas
                    Console.WriteLine("Associated row: " + commentRevision.Row);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Nota: Column es de solo lectura, por lo que no podemos modificarlo directamente
                    // Podemos cambiarlo indirectamente modificando CellName
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "E5"; // This will update both Row and Column properties
                    Console.WriteLine("After CellName change - New column: " + commentRevision.Column);
                    
                    // Restaurar el valor original
                    commentRevision.CellName = originalCellName;
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellCommentPropertyColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


