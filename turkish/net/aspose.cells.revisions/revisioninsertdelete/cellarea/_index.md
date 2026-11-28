---
title: "RevisionInsertDelete.CellArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionInsertDelete özelliği. Ekleme/silme aralığını alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioninsertdelete/cellarea/
---
## RevisionInsertDelete.CellArea property

Ekleme/silme aralığını alır.

```csharp
public CellArea CellArea { get; }
```

### Örnekler

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

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


