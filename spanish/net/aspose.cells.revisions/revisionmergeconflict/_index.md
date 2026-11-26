---
title: "Clase RevisionMergeConflict"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionMergeConflict. Representa un registro de revisión que indica que hubo un conflicto de fusión"
type: docs
url: /es/net/aspose.cells.revisions/revisionmergeconflict/
---
## RevisionMergeConflict class

Representa un registro de revisión que indica que hubo un conflicto de fusión.

```csharp
public class RevisionMergeConflict : Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión.(Heredado de [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionmergeconflict/type/) { get; } | Obtiene el tipo de revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. (Heradado de [`Revision`](../revision/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionsClassRevisionMergeConflictDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Realiza algunos cambios para crear historial de revisiones
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue("Another Value");

            // Guarda el libro de trabajo para generar revisiones
            workbook.Save("RevisionMergeConflictDemo_Before.xlsx");

            // Crea un escenario de conflicto de fusión
            worksheet.Cells["A1"].PutValue("Conflicting Change 1");
            worksheet.Cells["A1"].PutValue("Conflicting Change 2");

            // Obtén el historial de revisiones (itera directamente a través de RevisionLogCollection)
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Encuentra y demuestra RevisionMergeConflict
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionMergeConflict mergeConflict)
                    {
                        // Demostrar el acceso al tipo de revisión
                        RevisionType revisionType = mergeConflict.Type;
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionMergeConflictDemo_After.xlsx");
        }
    }
}
```

### Ver también

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


