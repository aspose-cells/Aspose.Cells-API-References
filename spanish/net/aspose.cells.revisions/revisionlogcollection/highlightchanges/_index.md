---
title: "RevisionLogCollection.HighlightChanges"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método RevisionLogCollection. Resalta los cambios del libro compartido"
type: docs
url: /es/net/aspose.cells.revisions/revisionlogcollection/highlightchanges/
---
## RevisionLogCollection.HighlightChanges method

Resalta los cambios del libro compartido.

```csharp
public void HighlightChanges(HighlightChangesOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | HighlightChangesOptions | Establecer las opciones para filtrar qué cambios deben ser rastreados. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionMethodHighlightChangesWithHighlightChangesOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo y revisiones
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Resaltar cambios con opciones
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            workbook.Worksheets.RevisionLogs.HighlightChanges(options);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


