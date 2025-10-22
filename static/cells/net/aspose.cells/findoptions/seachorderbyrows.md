##FindOptions.SeachOrderByRows
FindOptions property. Indicates whether search order by rows or columns
## FindOptions.SeachOrderByRows property
Indicates whether search order by rows or columns.
```csharp
[Obsolete("Use FindOptions.SearchOrderByRows property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SeachOrderByRows { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use FindOptions.SearchOrderByRows property. This property will be removed 12 months later since November 2018. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsPropertySeachOrderByRowsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
for (int row = 0; row < 10; row++)
{
for (int col = 0; col < 5; col++)
{
worksheet.Cells[row, col].PutValue($"Data_{row}_{col}");
}
}
// Add our search value at a specific location
worksheet.Cells[5, 2].PutValue("SearchTarget");
// Create find options
FindOptions findOptions = new FindOptions();
findOptions.SeachOrderByRows = true; // Search row by row
findOptions.LookInType = LookInType.Values;
findOptions.LookAtType = LookAtType.Contains;
// Find the cell
Cell foundCell = worksheet.Cells.Find("SearchTarget", null, findOptions);
if (foundCell != null)
{
Console.WriteLine($"Found at Row: {foundCell.Row}, Column: {foundCell.Column}");
}
else
{
Console.WriteLine("Value not found");
}
}
}
}
```
### See Also
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
