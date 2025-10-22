##Class RevisionLog
Aspose.Cells.Revisions.RevisionLog class. Represents the revision log
## RevisionLog class
Represents the revision log.
```csharp
public class RevisionLog
```
## Properties
| Name | Description |
| --- | --- |
| [MetadataTable](../../aspose.cells.revisions/revisionlog/metadatatable/) { get; } | Gets table that contains metadata about a list of specific changes that have taken place for this workbook. |
| [Revisions](../../aspose.cells.revisions/revisionlog/revisions/) { get; } | Gets all revisions in this log. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionLogDemo
{
public static void RevisionLogExample()
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
}
}
```
### See Also
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)
