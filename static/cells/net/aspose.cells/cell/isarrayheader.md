##Cell.IsArrayHeader
Cell property. Indicates the cells formula is an array formula and it is the first cell of the array
## Cell.IsArrayHeader property
Indicates the cell's formula is an array formula and it is the first cell of the array.
```csharp
public bool IsArrayHeader { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsArrayHeaderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create an array formula in range B2:D4
worksheet.Cells["B2"].SetArrayFormula("=A1:A3*B1:B3", 3, 3);
// Verify and print the IsArrayHeader property
// Note: IsArrayHeader is read-only and automatically set for array formula headers
Console.WriteLine("B2 IsArrayHeader: " + worksheet.Cells["B2"].IsArrayHeader);
Console.WriteLine("B3 IsArrayHeader: " + worksheet.Cells["B3"].IsArrayHeader);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
