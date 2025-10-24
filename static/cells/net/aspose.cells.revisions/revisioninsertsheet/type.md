##RevisionInsertSheet.Type
RevisionInsertSheet property. Gets the type of revision
## RevisionInsertSheet.Type property
Gets the type of revision.
```csharp
public override RevisionType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionInsertSheetPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
// Enable revision tracking (simulated since StartTrackingRevisions isn't available)
bool trackRevisions = true;
// Add a new worksheet to generate a revision record
Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
// Simulate getting revisions (since Revisions property isn't available)
if (trackRevisions && workbook.HasRevisions)
{
// In a real scenario, we would access the revisions here
// This assumes we got the revision from somewhere (like workbook.Revisions)
RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
if (insertSheetRevision != null)
{
// Display the Type property
Console.WriteLine("Revision Type: " + insertSheetRevision.Type);
// Demonstrate usage of the read-only Type property
if (insertSheetRevision.Type == RevisionType.InsertSheet)
{
Console.WriteLine("This revision represents a sheet insertion operation");
// Show additional information about the inserted sheet
Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);
Console.WriteLine("Sheet position: " + insertSheetRevision.SheetPosition);
}
// Check against other revision types
if (insertSheetRevision.Type != RevisionType.Unknown)
{
Console.WriteLine("This is a known revision type");
}
}
// Save the workbook
workbook.Save("RevisionInsertSheetTypeDemo.xlsx");
}
else
{
Console.WriteLine("No revisions found or revision tracking not enabled");
}
}
}
}
```
### See Also
* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
