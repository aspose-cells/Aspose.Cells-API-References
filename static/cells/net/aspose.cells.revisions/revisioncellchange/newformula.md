##RevisionCellChange.NewFormula
RevisionCellChange property. Gets the old formula
## RevisionCellChange.NewFormula property
Gets the old formula.
```csharp
public string NewFormula { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellChangePropertyNewFormulaDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set initial formula in cell A1
worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
// Change the formula to create a revision
worksheet.Cells["A1"].Formula = "=AVERAGE(B1:B3)";
// Access the revision logs
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
foreach (RevisionLog log in revisionLogs)
{
foreach (Revision revision in log.Revisions)
{
if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
{
// Display formula change information
Console.WriteLine("Cell Name: " + cellChange.CellName);
Console.WriteLine("Old Formula: " + cellChange.OldFormula);
Console.WriteLine("New Formula: " + cellChange.NewFormula);
Console.WriteLine("Old Value: " + cellChange.OldValue);
Console.WriteLine("New Value: " + cellChange.NewValue);
// Demonstrate using the NewFormula property
if (!string.IsNullOrEmpty(cellChange.NewFormula))
{
Console.WriteLine("\nThe cell's new formula calculates: " +
worksheet.Cells["A1"].StringValue);
}
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellChangePropertyNewFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
