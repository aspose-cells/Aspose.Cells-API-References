---
title: "RevisionCustomView.Guid"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCustomView-Eigenschaft. Gibt die global eindeutige Kennung der benutzerdefinierten Ansicht zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncustomview/guid/
---
## RevisionCustomView.Guid property

Ruft die global eindeutige Kennung der benutzerdefinierten Ansicht ab.

```csharp
public Guid Guid { get; }
```

### Beispiele

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
            // Öffne eine vorhandene Arbeitsmappe, die benutzerdefinierte Ansicht-Revisionen enthält
            Workbook workbook = new Workbook("example.xlsx");
            
            // Verarbeite Revisionsprotokolle
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

### Siehe auch

* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


