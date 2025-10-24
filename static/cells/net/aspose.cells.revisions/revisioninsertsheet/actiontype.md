##RevisionInsertSheet.ActionType
RevisionInsertSheet property. Gets the action type of the revision
## RevisionInsertSheet.ActionType property
Gets the action type of the revision.
```csharp
public RevisionActionType ActionType { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionInsertSheetPropertyActionTypeDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
// Note: StartTrackingRevisions is not available in the provided API
// workbook.StartTrackingRevisions();
// Add a new worksheet to generate a revision record
Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
// Note: StopTrackingRevisions is not available in the provided API
// workbook.StopTrackingRevisions();
// Note: Revisions property is not available in the provided API
// We'll use HasRevisions to check if there are any revisions
if (workbook.HasRevisions)
{
// In a real scenario, we would access the revisions here
// Since we can't create RevisionInsertSheet directly, we'll simulate checking one
// This assumes we got the revision from somewhere (like workbook.Revisions)
RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
// Since we can't create or set ActionType, we'll just demonstrate checking it
if (insertSheetRevision != null)
{
// Display the ActionType property
Console.WriteLine("ActionType of sheet insertion: " + insertSheetRevision.ActionType);
// Demonstrate usage of the read-only property
if (insertSheetRevision.ActionType == RevisionActionType.Add)
{
Console.WriteLine("This revision represents a sheet addition");
}
}
// Save the workbook with revisions
workbook.Save("RevisionInsertSheetActionTypeDemo.xlsx");
}
else
{
Console.WriteLine("No sheet insertion revision found");
}
}
}
}
```
### See Also
* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
