---
title: "RevisionInsertDelete.Revisions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionInsertDelete. Obtiene la lista de revisiones mediante esta operación"
type: docs
url: /es/net/aspose.cells.revisions/revisioninsertdelete/revisions/
---
## RevisionInsertDelete.Revisions property

Obtiene la lista de revisiones de esta operación.

```csharp
public RevisionCollection Revisions { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyRevisionsDemo
    {
        public static void Run()
        {
            // Cree un nuevo workbook y habilite el seguimiento de revisiones
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Realizar operaciones para generar revisiones
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteRows(1, 1);

            // Obtener los registros de revisiones
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Iterar a través de todos los registros de revisiones
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Acceder a la propiedad Revisions (solo lectura)
                        RevisionCollection revisions = revisionInsertDelete.Revisions;

                        // Mostrar información sobre las revisiones
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);
                        Console.WriteLine("Action Type: " + revisionInsertDelete.ActionType);
                        Console.WriteLine("Cell Area: " + revisionInsertDelete.CellArea);
                        Console.WriteLine("Number of related revisions: " + revisions.Count);

                        // Demostrar el uso de la colección Revisions
                        foreach (Revision relatedRevision in revisions)
                        {
                            Console.WriteLine(" - Related revision ID: " + relatedRevision.Id);
                            if (relatedRevision is RevisionInsertDelete)
                            {
                                RevisionInsertDelete relatedInsertDelete = (RevisionInsertDelete)relatedRevision;
                                Console.WriteLine("   Action Type: " + relatedInsertDelete.ActionType);
                                Console.WriteLine("   Cell Area: " + relatedInsertDelete.CellArea);
                            }
                        }
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionInsertDeletePropertyRevisionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


