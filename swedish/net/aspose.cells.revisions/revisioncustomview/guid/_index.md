---
title: "RevisionCustomView.Guid"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCustomView‑egenskapen. Hämtar den globalt unika identifieraren för den anpassade vyn"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncustomview/guid/
---
## RevisionCustomView.Guid property

Hämtar den globalt unika identifieraren för den anpassade vyn.

```csharp
public Guid Guid { get; }
```

### Exempel

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
            // Öppna en befintlig arbetsbok som innehåller anpassade vyrevisioner
            Workbook workbook = new Workbook("example.xlsx");
            
            // Bearbeta revisionsloggar
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

### Se även

* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


