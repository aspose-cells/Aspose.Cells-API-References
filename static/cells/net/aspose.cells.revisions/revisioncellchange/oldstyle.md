##RevisionCellChange.OldStyle
RevisionCellChange property. Gets the old style of the cell
## RevisionCellChange.OldStyle property
Gets the old style of the cell.
```csharp
public Style OldStyle { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellChangePropertyOldStyleDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set initial style for cell A1
Cell cell = worksheet.Cells["A1"];
Style initialStyle = workbook.CreateStyle();
initialStyle.Font.Name = "Arial";
initialStyle.Font.Size = 10;
initialStyle.Font.Color = System.Drawing.Color.Black;
cell.SetStyle(initialStyle);
cell.PutValue("Initial Value");
// Change the cell style to create a revision
Style newStyle = workbook.CreateStyle();
newStyle.Font.Name = "Times New Roman";
newStyle.Font.Size = 12;
newStyle.Font.Color = System.Drawing.Color.Red;
newStyle.Font.IsBold = true;
cell.SetStyle(newStyle);
cell.PutValue("Modified Value");
// Access the revision logs
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
foreach (RevisionLog log in revisionLogs)
{
foreach (Revision revision in log.Revisions)
{
if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
{
// Display style change information
Console.WriteLine("Cell Name: " + cellChange.CellName);
Console.WriteLine("Old Style Font: " + cellChange.OldStyle.Font.Name);
Console.WriteLine("Old Style Size: " + cellChange.OldStyle.Font.Size);
Console.WriteLine("Old Style Color: " + cellChange.OldStyle.Font.Color);
Console.WriteLine("New Style Font: " + cellChange.NewStyle.Font.Name);
Console.WriteLine("New Style Size: " + cellChange.NewStyle.Font.Size);
Console.WriteLine("New Style Color: " + cellChange.NewStyle.Font.Color);
// Demonstrate using the OldStyle property
if (cellChange.OldStyle.Font.Name == "Arial")
{
Console.WriteLine("\nThe cell originally had Arial font");
}
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellChangePropertyOldStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
