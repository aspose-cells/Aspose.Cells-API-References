---
title: "WorksheetCollection.RevisionLogs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Representa los registros de revisión"
type: docs
url: /es/net/aspose.cells/worksheetcollection/revisionlogs/
---
## WorksheetCollection.RevisionLogs property

Representa los registros de revisiones.

```csharp
public RevisionLogCollection RevisionLogs { get; }
```

### Ejemplos

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

### Ver también

* class [RevisionLogCollection](../../../aspose.cells.revisions/revisionlogcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


