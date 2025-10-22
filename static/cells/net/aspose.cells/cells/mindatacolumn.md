##Cells.MinDataColumn
Cells property. Minimum column index of cell which contains data
## Cells.MinDataColumn property
Minimum column index of cell which contains data.
```csharp
public int MinDataColumn { get; }
```
### Remarks
-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyMinDataColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add some data to cells (starting from column 2)
cells["B1"].PutValue("Header1");
cells["C2"].PutValue("Data1");
cells["D3"].PutValue("Data2");
cells["E4"].PutValue("Data3");
// Get the minimum column index that contains data
int minDataColumn = cells.MinDataColumn;
// Output the result
Console.WriteLine("Minimum data column index: " + minDataColumn);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
