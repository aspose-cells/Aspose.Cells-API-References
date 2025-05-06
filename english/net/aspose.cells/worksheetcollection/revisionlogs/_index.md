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
            // Create a new workbook
            Workbook workbook = new Workbook(&quot;HighlightedChangesWorkbook_original.xlsx&quot;);

            // Access the revision logs of the workbook
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Check if there are any revision logs
            if (revisionLogs.Count &gt; 0)
            {
                // Access the first revision log
                RevisionLog revisionLog = revisionLogs[0];

                // Access the metadata table of the revision log
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // Access the revisions in the revision log
                RevisionCollection revisions = revisionLog.Revisions;

                // Display some information about the revisions
                Console.WriteLine(&quot;Number of revisions: &quot; + revisions.Count);
                Console.WriteLine(&quot;Metadata Table: &quot; + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine(&quot;No revision logs found.&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;RevisionLogExample.xlsx&quot;);
        }
```

### See Also

* class [RevisionLogCollection](../../../aspose.cells.revisions/revisionlogcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


