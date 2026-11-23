---
title: "Revision.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Revision. Représente le type de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revision/type/
---
## Revision.Type property

Représente le type de révision.

```csharp
public virtual RevisionType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook("example.xlsx");
            if (!wb.HasRevisions)
            {
                Console.WriteLine("No revisions found");
                return;
            }

            foreach (RevisionLog log in wb.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange change = (RevisionCellChange)rv;
                        Console.WriteLine($"Cell {change.CellName} (Row {change.Row}):");
                        Console.WriteLine($"Old formula: {change.OldFormula ?? "N/A"}");
                    }
                }
            }
        }
    }
}
```

### Voir aussi

* enum [RevisionType](../../revisiontype/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


