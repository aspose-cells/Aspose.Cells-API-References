---
title: "Clase RevisionAutoFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionAutoFormat. representa un registro de revisión de información sobre un cambio de formato"
type: docs
url: /es/net/aspose.cells.revisions/revisionautoformat/
---
## RevisionAutoFormat class

Representa un registro de revisión de información sobre un cambio de formato.

```csharp
public class RevisionAutoFormat : Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionautoformat/cellarea/) { get; } | Obtiene la ubicación donde se aplicó el formato. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión.(Heredado de [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionautoformat/type/) { get; } | Obtiene el tipo de la revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. (Heradado de [`Revision`](../revision/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionAutoFormatDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();

            try
            {
                // Accede a la colección de registros de revisión
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Encuentra la primera instancia de RevisionAutoFormat
                RevisionAutoFormat revisionFormat = null;
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionAutoFormat)
                        {
                            revisionFormat = (RevisionAutoFormat)revision;
                            break;
                        }
                    }
                    if (revisionFormat != null) break;
                }

                if (revisionFormat != null)
                {
                    // Demuestra la propiedad Type (solo lectura)
                    RevisionType type = revisionFormat.Type;
                    Console.WriteLine($"Revision type: {type}");

                    // Demuestra la propiedad CellArea (solo lectura)
                    CellArea area = revisionFormat.CellArea;
                    Console.WriteLine($"Formatting applied to area: StartRow={area.StartRow}, " +
                                      $"StartColumn={area.StartColumn}, EndRow={area.EndRow}, " +
                                      $"EndColumn={area.EndColumn}");
                }
                else
                {
                    Console.WriteLine("No auto-format revisions found in the workbook");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionAutoFormat: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


