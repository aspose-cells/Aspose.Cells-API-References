---
title: "WorksheetCollection.RevisionLogs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorksheetCollection. Rappresenta i log di revisione"
type: docs
url: /it/net/aspose.cells/worksheetcollection/revisionlogs/
---
## WorksheetCollection.RevisionLogs property

Rappresenta i registri di revisione.

```csharp
public RevisionLogCollection RevisionLogs { get; }
```

### Esempi

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

### Vedi anche

* class [RevisionLogCollection](../../../aspose.cells.revisions/revisionlogcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


