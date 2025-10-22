##Cell.Worksheet
Cell property. Gets the parent worksheet
## Cell.Worksheet property
Gets the parent worksheet.
```csharp
public Worksheet Worksheet { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyWorksheetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue(100);
worksheet.Cells["A2"].PutValue(200);
worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
// Access a cell and demonstrate Worksheet property
Cell cell = worksheet.Cells["A3"];
// Display worksheet information through cell's Worksheet property
Console.WriteLine("Cell A3 is in worksheet: " + cell.Worksheet.Name);
Console.WriteLine("Calculation result in A3: " + cell.Value);
// Add another worksheet and demonstrate cross-sheet reference
Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
sheet2.Cells["B1"].PutValue("=A3");
// Access the cell in Sheet2 and show its worksheet
Cell crossSheetCell = sheet2.Cells["B1"];
Console.WriteLine("Cell B1 is in worksheet: " + crossSheetCell.Worksheet.Name);
Console.WriteLine("Cross-sheet reference in B1: " + crossSheetCell.Value);
}
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
