---
title: WorksheetCollection.RevisionLogs
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Represents revision logs
type: docs
url: /net/aspose.cells/worksheetcollection/revisionlogs/
---
## WorksheetCollection.RevisionLogs property

Represents revision logs.

```csharp
public RevisionLogCollection RevisionLogs { get; }
```

### Examples

```csharp
// Called: RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
public static void Property_RevisionLogs()
        {
            // Instantiate a Workbook object
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Get the revision logs
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Set the number of days to preserve the history
            revisionLogs.DaysPreservingHistory = 30;

            // Create HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // Highlight changes
            revisionLogs.HighlightChanges(options);

            // Save the workbook with highlighted changes
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
```

### See Also

* class [RevisionLogCollection](../../../aspose.cells.revisions/revisionlogcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


