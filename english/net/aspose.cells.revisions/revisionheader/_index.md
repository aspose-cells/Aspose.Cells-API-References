---
title: Class RevisionHeader
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionHeader class. Represents a list of specific changes that have taken place for this workbook
type: docs
url: /net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

Represents a list of specific changes that have taken place for this workbook.

```csharp
public class RevisionHeader
```

## Constructors

| Name | Description |
| --- | --- |
| [RevisionHeader](revisionheader/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | Gets and sets rhe date and time when this set of revisions was saved. |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | Gets and sets the name of the user making the revision. |

### Examples

```csharp
// Called: RevisionHeader metadataTable = revisionLog.MetadataTable;
public static void Type_RevisionHeader()
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

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


