##PasteOptions.OnlyVisibleCells
PasteOptions property. True means only copying visible cells
## PasteOptions.OnlyVisibleCells property
True means only copying visible cells.
```csharp
public bool OnlyVisibleCells { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PasteOptionsPropertyOnlyVisibleCellsDemo
{
public static void Run()
{
// Create a workbook with two worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add();
// Get cells from first worksheet and populate data
Cells sourceCells = workbook.Worksheets[0].Cells;
sourceCells["A1"].PutValue("Hidden A1");
sourceCells["B2"].PutValue("Visible B2");
sourceCells["C3"].PutValue("Hidden C3");
// Hide some rows and columns
sourceCells.HideRow(0);  // Hides row 1 (A1)
sourceCells.HideColumn(2); // Hides column C (C3)
// Create source range to copy
Aspose.Cells.Range sourceRange = sourceCells.CreateRange("A1:C3");
// Get cells from second worksheet for destination
Cells destCells = workbook.Worksheets[1].Cells;
Aspose.Cells.Range destRange = destCells.CreateRange("A1:C3");
// Create paste options and set OnlyVisibleCells
PasteOptions pasteOptions = new PasteOptions();
pasteOptions.OnlyVisibleCells = true;
// Copy only visible cells
destRange.Copy(sourceRange, pasteOptions);
// Output results to demonstrate functionality
Console.WriteLine("B2 value (should be copied): " + destCells["B2"].StringValue);
Console.WriteLine("A1 value (should be empty): " + destCells["A1"].StringValue);
Console.WriteLine("C3 value (should be empty): " + destCells["C3"].StringValue);
}
}
}
```
### See Also
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
