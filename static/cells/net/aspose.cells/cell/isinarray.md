##Cell.IsInArray
Cell property. Indicates whether the cell formula is an array formula
## Cell.IsInArray property
Indicates whether the cell formula is an array formula.
```csharp
[Obsolete("Use IsArrayFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInArray { get; }
```
### Remarks
NOTE: This class is now obsolete. Instead, please use Cell.IsArrayFormula to check whether the cell formula is an array formula. This property will be removed 12 months later since May 2018. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsInArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data with array formulas
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["B3"].PutValue(40);
// Set an array formula using the correct API
worksheet.Cells["C2"].SetArrayFormula("A2:A3*B2:B3", 2, 1);
// Check IsInArray property
Cell cellInArray = worksheet.Cells["C2"];
Cell cellNotInArray = worksheet.Cells["A2"];
Console.WriteLine("Cell C2 is in array: " + cellInArray.IsInArray);
Console.WriteLine("Cell A2 is in array: " + cellNotInArray.IsInArray);
// Demonstrate clearing non-array cells
for (int row = 1; row <= 3; row++)
{
for (int col = 0; col < 3; col++)
{
Cell cell = worksheet.Cells[row, col];
if (!cell.IsInArray && !cell.IsFormula)
{
cell.PutValue("");
}
}
}
// Save the workbook
workbook.Save("IsInArrayDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
