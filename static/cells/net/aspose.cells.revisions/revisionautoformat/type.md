##RevisionAutoFormat.Type
RevisionAutoFormat property. Gets the type of the revision
## RevisionAutoFormat.Type property
Gets the type of the revision.
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
public class RevisionAutoFormatPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
try
{
// Access the revision logs collection
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
// Find the first RevisionAutoFormat instance
RevisionAutoFormat revisionFormat = null;
foreach (RevisionLog revisionLog in revisionLogs)
{
foreach (Revision revision in revisionLog.Revisions)
{
if (revision is RevisionAutoFormat)
{
revisionFormat = (RevisionAutoFormat)revision;
break;
}
}
if (revisionFormat != null) break;
}
if (revisionFormat != null)
{
// Demonstrate the Type property (read-only)
RevisionType type = revisionFormat.Type;
Console.WriteLine($"Revision type: {type}");
// Show the enum value for clarity
Console.WriteLine($"Revision type value: {(int)type}");
}
else
{
Console.WriteLine("No auto-format revisions found in the workbook");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* enum [RevisionType](../../revisiontype/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
