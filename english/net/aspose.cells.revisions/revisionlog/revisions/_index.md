---
title: RevisionLog.Revisions
second_title: Aspose.Cells for .NET API Reference
description: RevisionLog property. Gets all revisions in this log
type: docs
url: /net/aspose.cells.revisions/revisionlog/revisions/
---
## RevisionLog.Revisions property

Gets all revisions in this log.

```csharp
public RevisionCollection Revisions { get; }
```

### Examples

```csharp
// Called: RevisionCollection revisions = revisionLog.Revisions;
public static void Property_Revisions()
        {
            // Create a new workbook
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Access the revision logs of the workbook
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Check if there are any revision logs
            if (revisionLogs.Count > 0)
            {
                // Access the first revision log
                RevisionLog revisionLog = revisionLogs[0];

                // Access the metadata table of the revision log
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // Access the revisions in the revision log
                RevisionCollection revisions = revisionLog.Revisions;

                // Display some information about the revisions
                Console.WriteLine("Number of revisions: " + revisions.Count);
                Console.WriteLine("Metadata Table: " + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine("No revision logs found.");
            }

            // Save the workbook
            workbook.Save("RevisionLogExample.xlsx");
        }
```

### See Also

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


