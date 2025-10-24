##Revision.Worksheet
Revision property. Gets the worksheet
## Revision.Worksheet property
Gets the worksheet.
```csharp
public Worksheet Worksheet { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionPropertyWorksheetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set worksheet properties
worksheet.Name = "Demo Sheet";
worksheet.IsGridlinesVisible = true;
worksheet.DisplayZeros = false;
worksheet.Zoom = 120;
// Add some data to demonstrate revisions
worksheet.Cells["A1"].PutValue("Original Value");
// Protect the worksheet to enable tracking changes
worksheet.Protect(ProtectionType.All);
// Make a change that will be tracked as revision
worksheet.Cells["A1"].PutValue("Modified Value");
// Save the workbook to track revisions
workbook.Save("RevisionDemo.xlsx");
// Load the workbook with revisions
Workbook workbookWithRevisions = new Workbook("RevisionDemo.xlsx");
// Access revision logs
foreach (RevisionLog log in workbookWithRevisions.Worksheets.RevisionLogs)
{
foreach (Revision revision in log.Revisions)
{
// Demonstrate accessing Worksheet property from revision
Console.WriteLine($"Revision Type: {revision.Type}");
Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");
Console.WriteLine($"Worksheet Index: {revision.Worksheet.Index}");
if (revision.Type == RevisionType.ChangeCells)
{
RevisionCellChange cellChange = (RevisionCellChange)revision;
Console.WriteLine($"Cell changed in worksheet '{cellChange.Worksheet.Name}': {cellChange.CellName}");
}
}
}
}
}
}
```
### See Also
* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
