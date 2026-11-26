---
title: "WorksheetCollection.RevisionLogs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Представляет журналы правок"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/revisionlogs/
---
## WorksheetCollection.RevisionLogs property

Представляет журналы ревизий.

```csharp
public RevisionLogCollection RevisionLogs { get; }
```

### Примеры

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

### См. также

* class [RevisionLogCollection](../../../aspose.cells.revisions/revisionlogcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


