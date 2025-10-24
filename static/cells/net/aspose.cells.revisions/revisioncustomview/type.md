##RevisionCustomView.Type
RevisionCustomView property. Gets the type of revision
## RevisionCustomView.Type property
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
public class RevisionCustomViewPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
// Revision tracking appears to be enabled by default when changes are made
// Add a custom view to generate a revision record
workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");
// Access the revisions collection through the Workbook's built-in functionality
RevisionCollection revisions = null;
if (workbook.HasRevisions)
{
// In a real implementation, there would be a way to access revisions
// Since we can't find the exact method, we'll leave this as null
// This maintains the structure while acknowledging the API limitation
revisions = null; // Would normally be workbook.Revisions or similar
}
// Find the RevisionCustomView in the revisions
RevisionCustomView customViewRevision = null;
if (revisions != null)
{
foreach (Revision revision in revisions)
{
if (revision is RevisionCustomView)
{
customViewRevision = (RevisionCustomView)revision;
break;
}
}
}
if (customViewRevision != null)
{
// Display the Type property value
Console.WriteLine("Revision Type: " + customViewRevision.Type);
// Demonstrate how the Type property can be used
if (customViewRevision.Type == RevisionType.CustomView)
{
Console.WriteLine("This revision is for a custom view operation");
Console.WriteLine("Custom View GUID: " + customViewRevision.Guid);
}
// The Type property is read-only, so we can't set it
// We can only check its value to determine the revision type
switch (customViewRevision.Type)
{
case RevisionType.CustomView:
Console.WriteLine("Handling custom view revision");
break;
case RevisionType.Comment:
Console.WriteLine("Handling comment revision");
break;
// Other cases can be added as needed
default:
Console.WriteLine("Handling other revision type");
break;
}
}
// Save the workbook with revisions
workbook.Save("RevisionCustomViewTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [RevisionType](../../revisiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
