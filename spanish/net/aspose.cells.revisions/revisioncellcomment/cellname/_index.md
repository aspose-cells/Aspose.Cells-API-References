---
title: "RevisionCellComment.CellName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCellComment. Obtiene el nombre de la celda"
type: docs
url: /es/net/aspose.cells.revisions/revisioncellcomment/cellname/
---
## RevisionCellComment.CellName property

Obtiene el nombre de la celda.

```csharp
public string CellName { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyCellNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda B5
            int commentRow = 4;
            int commentCol = 1;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Modificar el comentario para generar una revisión
            comment.Note = "Updated comment";

            // Accede a las revisiones
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Mostrar el valor actual de CellName
                    Console.WriteLine("Original CellName: " + commentRevision.CellName);
                    
                    // Cambiar la propiedad CellName
                    commentRevision.CellName = "C10";
                    Console.WriteLine("Modified CellName: " + commentRevision.CellName);
                    
                    // Demostrar el efecto de cambiar CellName
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    
                    // Nota: Cambiar CellName actualiza las propiedades Row/Column
                    Console.WriteLine("After CellName change - Row: " + commentRevision.Row);
                    Console.WriteLine("After CellName change - Column: " + commentRevision.Column);
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCellCommentPropertyCellNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


