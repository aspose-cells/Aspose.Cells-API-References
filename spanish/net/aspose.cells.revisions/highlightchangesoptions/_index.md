---
title: "Clase HighlightChangesOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.HighlightChangesOptions. Representa opciones de resaltado de revisiones o cambios de archivos Excel compartidos"
type: docs
url: /es/net/aspose.cells.revisions/highlightchangesoptions/
---
## HighlightChangesOptions class

Representa opciones de resaltado de revisiones o cambios de archivos de Excel compartidos.

```csharp
public class HighlightChangesOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HighlightChangesOptions](highlightchangesoptions/)(bool, bool) | Representa opciones de resaltado de revisiones o cambios de archivos de Excel compartidos. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsDemo
    {
        public static void HighlightChangesExample()
        {
            // Instanciar un objeto Workbook
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Obtener los registros de revisiones
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Establecer el número de días para conservar el historial
            revisionLogs.DaysPreservingHistory = 30;

            // Crear HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // Resaltar cambios
            revisionLogs.HighlightChanges(options);

            // Guarda el libro de trabajo con los cambios resaltados
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


