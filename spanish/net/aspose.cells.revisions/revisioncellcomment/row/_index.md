---
title: "RevisionCellComment.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellComment. Obtiene el índice de fila del que contiene un comentario"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellcomment/row/
---
## RevisionCellComment.Row property

Obtiene el índice de fila que contiene un comentario

```csharp
public int Row { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade un comentario a la celda D4 (fila 3, columna 3)
            int commentRow = 3;
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
                    
                    // Muestra el valor de la propiedad Row
                    Console.WriteLine("Comment is located at row: " + commentRevision.Row);
                    
                    // Demuestra el uso de la propiedad Row
                    Console.WriteLine("Comment location details:");
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Muestra que Row es de solo lectura al intentar modificarla (generará un error de compilación)
                    // commentRevision.Row = 5; // Esta línea está comentada ya que Row es de solo lectura
                    
                    // Forma alternativa de cambiar la posición modificando CellName
                    Console.WriteLine("\nChanging comment position via CellName...");
                    commentRevision.CellName = "F10"; // Changes to row 9, column 5
                    Console.WriteLine("New Row index: " + commentRevision.Row);
                    Console.WriteLine("New Column index: " + commentRevision.Column);
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellCommentPropertyRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


