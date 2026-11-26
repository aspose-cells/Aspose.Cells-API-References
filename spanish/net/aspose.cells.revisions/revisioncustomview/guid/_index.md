---
title: "RevisionCustomView.Guid"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCustomView. Obtiene el identificador único global de la vista personalizada"
type: docs
url: /es/net/aspose.cells.revisions/revisioncustomview/guid/
---
## RevisionCustomView.Guid property

Obtiene el identificador único global de la vista personalizada.

```csharp
public Guid Guid { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCustomViewPropertyGuidDemo
    {
        public static void Run()
        {
            // Abrir un libro de trabajo existente que contiene revisiones de vista personalizada
            Workbook workbook = new Workbook("example.xlsx");
            
            // Procesar registros de revisión
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.CustomView)
                    {
                        RevisionCustomView rcv = (RevisionCustomView)revision;
                        Console.WriteLine($"ActionType: {rcv.ActionType}, Guid: {rcv.Guid}");
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


