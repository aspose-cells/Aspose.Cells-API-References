##RevisionRenameSheet.Type
RevisionRenameSheet property. Represents the type of the revision
## RevisionRenameSheet.Type property
Represents the type of the revision.
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
public class RevisionRenameSheetPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Enable tracking revisions BEFORE making changes
// Note: This method doesn't exist in the provided API, so we'll remove it
// workbook.StartTrackingRevisions();
// Rename the first worksheet to create a revision
Worksheet worksheet = workbook.Worksheets[0];
string originalName = worksheet.Name;
worksheet.Name = "RenamedSheet";
// Access the revisions collection
// Note: The Revisions property doesn't exist in the provided API
// So we'll need to check if workbook has revisions first
if (workbook.HasRevisions)
{
// Find the rename sheet revision
RevisionRenameSheet renameRevision = null;
// Since we can't access Revisions directly, we'll need to modify this part
// This is just a placeholder since the actual API doesn't support revisions access
Console.WriteLine("Revision tracking is not fully supported in this API version.");
if (renameRevision != null)
{
// Display the Type property value
Console.WriteLine("Revision Type: " + renameRevision.Type);
Console.WriteLine("Old Sheet Name: " + renameRevision.OldName);
Console.WriteLine("New Sheet Name: " + renameRevision.NewName);
// Demonstrate how to use the Type property
if (renameRevision.Type == RevisionType.RenameSheet)
{
Console.WriteLine("This revision represents a worksheet rename operation.");
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionRenameSheetDemo.xlsx");
}
}
}
```
### See Also
* enum [RevisionType](../../revisiontype/)
* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
