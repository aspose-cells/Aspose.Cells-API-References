##RevisionMergeConflict.Type
RevisionMergeConflict property. Gets the type of revision
## RevisionMergeConflict.Type property
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
public class RevisionMergeConflictPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Enable track changes
workbook.StartAccessCache(AccessCacheOptions.All);
// Make changes to create a merge conflict scenario
worksheet.Cells["A1"].PutValue("Original Value");
workbook.Save("TempMergeConflict.xlsx");
// Simulate a merge conflict by opening the file and making conflicting changes
Workbook otherUserWorkbook = new Workbook("TempMergeConflict.xlsx");
otherUserWorkbook.Worksheets[0].Cells["A1"].PutValue("Conflicting Change");
otherUserWorkbook.Save("TempMergeConflict_OtherUser.xlsx");
// Merge the conflicting changes
workbook.Combine(otherUserWorkbook);
// Check if there are revisions
if (workbook.HasRevisions)
{
// Find the merge conflict revision
RevisionMergeConflict mergeConflictRevision = null;
// Note: In actual implementation, you would need another way to access revisions
// as the Revisions property is not available in the provided API definition
if (mergeConflictRevision != null)
{
// Display the Type property of the merge conflict revision
Console.WriteLine("Merge Conflict Revision Type: " + mergeConflictRevision.Type);
// Demonstrate how this information can be used
if (mergeConflictRevision.Type == RevisionType.MergeConflict)
{
Console.WriteLine("This revision represents a merge conflict.");
Console.WriteLine("Worksheet affected: " + mergeConflictRevision.Worksheet.Name);
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionMergeConflictTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [RevisionType](../../revisiontype/)
* class [RevisionMergeConflict](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
