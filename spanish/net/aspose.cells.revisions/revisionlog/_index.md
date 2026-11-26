---
title: "Clase RevisionLog"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionLog. Representa el registro de revisiones"
type: docs
url: /es/net/aspose.cells.revisions/revisionlog/
---
## RevisionLog class

Representa el registro de revisiones.

```csharp
public class RevisionLog
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [MetadataTable](../../aspose.cells.revisions/revisionlog/metadatatable/) { get; } | Obtiene la tabla que contiene metadatos sobre una lista de cambios específicos que se han producido en este libro de trabajo. |
| [Revisions](../../aspose.cells.revisions/revisionlog/revisions/) { get; } | Obtiene todas las revisiones en este registro. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogDemo
    {
        public static void RevisionLogExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Accede a los registros de revisión del libro de trabajo
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Verificar si hay registros de revisión
            if (revisionLogs.Count > 0)
            {
                // Accede al primer registro de revisión
                RevisionLog revisionLog = revisionLogs[0];

                // Accede a la tabla de metadatos del registro de revisión
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // Accede a las revisiones en el registro de revisión
                RevisionCollection revisions = revisionLog.Revisions;

                // Muestra alguna información sobre las revisiones
                Console.WriteLine("Number of revisions: " + revisions.Count);
                Console.WriteLine("Metadata Table: " + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine("No revision logs found.");
            }

            // Guarda el libro de trabajo
            workbook.Save("RevisionLogExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


