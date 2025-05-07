---
title: RevisionLog.MetadataTable
second_title: Aspose.Cells for .NET API Reference
description: RevisionLog property. Gets table that contains metadata about a list of specific changes that have taken place for this workbook
type: docs
url: /net/aspose.cells.revisions/revisionlog/metadatatable/
---
## RevisionLog.MetadataTable property

Gets table that contains metadata about a list of specific changes that have taken place for this workbook.

```csharp
public RevisionHeader MetadataTable { get; }
```

### Examples

```csharp
// Called: RevisionHeader metadataTable = revisionLog.MetadataTable;
public static void Property_MetadataTable()
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

* class [RevisionHeader](../../revisionheader/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


