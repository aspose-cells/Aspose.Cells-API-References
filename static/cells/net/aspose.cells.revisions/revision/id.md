##Revision.Id
Revision property. Gets the number of this revision
## Revision.Id property
Gets the number of this revision.
```csharp
public int Id { get; }
```
### Remarks
Zero means this revision does not contains id.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionPropertyIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Make a change to potentially create a revision
worksheet.Cells["A1"].Value = "Sample Data";
try
{
// Get the revision logs collection
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
if (revisionLogs != null && revisionLogs.Count > 0)
{
// Get revisions from the first log
RevisionCollection revisions = revisionLogs[0].Revisions;
if (revisions != null && revisions.Count > 0)
{
// Access the first revision
Revision revision = revisions[0];
// Display the Id property (read-only)
Console.WriteLine("Revision Id: " + revision.Id);
// Save the workbook
workbook.Save("RevisionIdDemo.xlsx");
}
else
{
Console.WriteLine("No revisions found in the log");
}
}
else
{
Console.WriteLine("No revision logs were created");
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
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
