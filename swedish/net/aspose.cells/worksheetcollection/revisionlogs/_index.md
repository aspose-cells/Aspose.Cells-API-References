---
title: "WorksheetCollection.RevisionLogs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Representerar revisionsloggar"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/revisionlogs/
---
## WorksheetCollection.RevisionLogs property

Representerar revisionsloggar.

```csharp
public RevisionLogCollection RevisionLogs { get; }
```

### Exempel

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

### Se även

* class [RevisionLogCollection](../../../aspose.cells.revisions/revisionlogcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


