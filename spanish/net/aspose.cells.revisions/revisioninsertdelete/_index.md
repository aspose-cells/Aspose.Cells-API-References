---
title: "Clase RevisionInsertDelete"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionInsertDelete. Representa un registro de revisión de una acción de inserción/eliminación de fila/columna"
type: docs
url: /es/net/aspose.cells.revisions/revisioninsertdelete/
---
## RevisionInsertDelete class

Representa un registro de revisión de una acción de inserción/eliminación de fila/columna.

```csharp
public class RevisionInsertDelete : Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertdelete/actiontype/) { get; } | Obtiene el tipo de acción de esta revisión. |
| [CellArea](../../aspose.cells.revisions/revisioninsertdelete/cellarea/) { get; } | Obtiene el rango de inserción/eliminación. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión.(Heredado de [`Revision`](../revision/).) |
| [Revisions](../../aspose.cells.revisions/revisioninsertdelete/revisions/) { get; } | Obtiene la lista de revisiones de esta operación. |
| override [Type](../../aspose.cells.revisions/revisioninsertdelete/type/) { get; } | Representa el tipo de revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. (Heradado de [`Revision`](../revision/).) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionsClassRevisionInsertDeleteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteColumn(0);

            string filePath = "RevisionsDemo.xlsx";
            workbook.Save(filePath);

            Workbook reopenedWorkbook = new Workbook(filePath);
            foreach (RevisionLog log in reopenedWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.InsertDelete)
                    {
                        RevisionInsertDelete rid = (RevisionInsertDelete)revision;
                        Console.WriteLine($"ActionType: {rid.ActionType}, CellArea: {rid.CellArea}");
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


