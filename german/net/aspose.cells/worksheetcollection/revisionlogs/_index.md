---
title: "WorksheetCollection.RevisionLogs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Stellt Revisionsprotokolle dar"
type: docs
url: /de/net/aspose.cells/worksheetcollection/revisionlogs/
---
## WorksheetCollection.RevisionLogs property

Stellt Revisionsprotokolle dar.

```csharp
public RevisionLogCollection RevisionLogs { get; }
```

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyRevisionLogsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Original");
            sheet.Cells["A1"].PutValue("Revised");

            workbook.Worksheets.RevisionLogs.HighlightChanges(new HighlightChangesOptions(true, true));
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [RevisionLogCollection](../../../aspose.cells.revisions/revisionlogcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


