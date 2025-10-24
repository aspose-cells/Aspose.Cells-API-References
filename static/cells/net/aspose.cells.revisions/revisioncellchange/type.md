##RevisionCellChange.Type
RevisionCellChange property. Represents the type of revision
## RevisionCellChange.Type property
Represents the type of revision.
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
public class RevisionCellChangePropertyTypeDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Enable track changes by modifying a cell - revisions are automatically tracked
// when changes are made after workbook creation
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Initial Value");
// Change the cell to create a revision
cell.PutValue("Modified Value");
// Access the revision logs
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
foreach (RevisionLog log in revisionLogs)
{
foreach (Revision revision in log.Revisions)
{
if (revision is RevisionCellChange cellChange)
{
// Display Type information from the revision
Console.WriteLine("Cell Name: " + cellChange.CellName);
Console.WriteLine("Revision Type: " + cellChange.Type);
// Demonstrate using the Type property
if (cellChange.Type == RevisionType.ChangeCells)
{
Console.WriteLine("\nThis is a cell change revision");
Console.WriteLine("Old Value: " + cellChange.OldValue);
Console.WriteLine("New Value: " + cellChange.NewValue);
}
// Check other possible revision types
switch (cellChange.Type)
{
case RevisionType.ChangeCells:
Console.WriteLine("Handling cell value change revision");
break;
case RevisionType.Format:
Console.WriteLine("Handling format change revision");
break;
default:
Console.WriteLine("Handling other type of revision");
break;
}
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellChangePropertyTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [RevisionType](../../revisiontype/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
