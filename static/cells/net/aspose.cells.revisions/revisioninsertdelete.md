##Class RevisionInsertDelete
Aspose.Cells.Revisions.RevisionInsertDelete class. Represents a revision record of a row/column insert/delete action
## RevisionInsertDelete class
Represents a revision record of a row/column insert/delete action.
```csharp
public class RevisionInsertDelete : Revision
```
## Properties
| Name | Description |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertdelete/actiontype/) { get; } | Gets the action type of this revision. |
| [CellArea](../../aspose.cells.revisions/revisioninsertdelete/cellarea/) { get; } | Gets the inserting/deleting range. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| [Revisions](../../aspose.cells.revisions/revisioninsertdelete/revisions/) { get; } | Gets revision list by this operation. |
| override [Type](../../aspose.cells.revisions/revisioninsertdelete/type/) { get; } | Represents the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionsClassRevisionInsertDeleteDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Settings.Shared = true;
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells.InsertRow(0);
worksheet.Cells.DeleteColumn(0);
string filePath = "RevisionsDemo.xlsx";
workbook.Save(filePath);
Workbook reopenedWorkbook = new Workbook(filePath);
foreach (RevisionLog log in reopenedWorkbook.Worksheets.RevisionLogs)
{
foreach (Revision revision in log.Revisions)
{
if (revision.Type == RevisionType.InsertDelete)
{
RevisionInsertDelete rid = (RevisionInsertDelete)revision;
Console.WriteLine($"ActionType: {rid.ActionType}, CellArea: {rid.CellArea}");
}
}
}
}
}
}
```
### See Also
* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)
