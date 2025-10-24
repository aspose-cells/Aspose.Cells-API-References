##ListObject.UpdateColumnName
ListObject method. Updates all list columns name from the worksheet
## ListObject.UpdateColumnName method
Updates all list columns' name from the worksheet.
```csharp
public void UpdateColumnName()
```
### Remarks
The value of the cells in the header row of the table must be same as the name of the ListColumn; Cell.PutValue do not auto modify the name of the ListColumn for performance.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ListObjectMethodUpdateColumnNameDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Create a table/list object
var listObject = ws.ListObjects[ws.ListObjects.Add(3, 3, 6, 6, true)];
// Populate some data in the table
for (int r = 0; r < 3; r++)
{
for (int c = 0; c < 3; c++)
{
if (c > 0)
ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue(r + c);
else
ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue("");
}
}
// Update column names (will set default names like Column1, Column2 etc.)
listObject.UpdateColumnName();
// Save the workbook
wb.Save("output.xlsx");
// Verify the column name was updated
Console.WriteLine("First column name: " + ws.Cells[listObject.StartRow, listObject.StartColumn].StringValue);
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
