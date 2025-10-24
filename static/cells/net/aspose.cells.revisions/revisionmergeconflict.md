##Class RevisionMergeConflict
Aspose.Cells.Revisions.RevisionMergeConflict class. Represents a revision record which indicates that there was a merge conflict
## RevisionMergeConflict class
Represents a revision record which indicates that there was a merge conflict.
```csharp
public class RevisionMergeConflict : Revision
```
## Properties
| Name | Description |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionmergeconflict/type/) { get; } | Gets the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
public class RevisionsClassRevisionMergeConflictDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Make some changes to create revision history
worksheet.Cells["A1"].PutValue("Original Value");
worksheet.Cells["A2"].PutValue("Another Value");
// Save the workbook to generate revisions
workbook.Save("RevisionMergeConflictDemo_Before.xlsx");
// Create a merge conflict scenario
worksheet.Cells["A1"].PutValue("Conflicting Change 1");
worksheet.Cells["A1"].PutValue("Conflicting Change 2");
// Get the revision history (iterate directly through RevisionLogCollection)
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
// Find and demonstrate RevisionMergeConflict
foreach (RevisionLog revisionLog in revisionLogs)
{
foreach (Revision revision in revisionLog.Revisions)
{
if (revision is RevisionMergeConflict mergeConflict)
{
// Demonstrate accessing the revision type
RevisionType revisionType = mergeConflict.Type;
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionMergeConflictDemo_After.xlsx");
}
}
}
```
### See Also
* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)
