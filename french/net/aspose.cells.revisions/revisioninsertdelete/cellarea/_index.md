---
title: "RevisionInsertDelete.CellArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionInsertDelete. Obtient la plage d’insertion/suppression"
type: docs
url: /fr/net/aspose.cells.revisions/revisioninsertdelete/cellarea/
---
## RevisionInsertDelete.CellArea property

Obtient la plage d'insertion/suppression.

```csharp
public CellArea CellArea { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionInsertDeletePropertyCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.InsertRow(0);
            workbook.Save("output.xlsx");

            Workbook reopened = new Workbook("output.xlsx");
            foreach (RevisionLog log in reopened.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.InsertDelete)
                    {
                        RevisionInsertDelete rrc = (RevisionInsertDelete)revision;
                        Console.WriteLine("ActionType: {0}; CellArea: {1}", rrc.ActionType, rrc.CellArea);
                    }
                }
            }
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


