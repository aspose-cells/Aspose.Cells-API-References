##ListColumn.Range
ListColumn property. Gets the range of this list column
## ListColumn.Range property
Gets the range of this list column.
```csharp
public Range Range { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListColumnPropertyRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a list object
worksheet.Cells["A1"].PutValue("Column1");
for (int i = 2; i <= 5; i++)
{
worksheet.Cells["A" + i].PutValue("Item " + i);
}
// Create a list object
int idx = worksheet.ListObjects.Add(0, 0, 4, 0, true);
ListObject listObj = worksheet.ListObjects[idx];
// Get the first list column
ListColumn listCol = listObj.ListColumns[0];
// Access the range of the list column
Aspose.Cells.Range range = listCol.Range;
// Display range information
Console.WriteLine("Range address: " + range.Address);
Console.WriteLine("Row count: " + range.RowCount);
Console.WriteLine("Column count: " + range.ColumnCount);
// Modify cells in the range
for (int i = 0; i < range.RowCount; i++)
{
range[i, 0].PutValue("Modified " + (i + 1));
}
// Save the workbook
workbook.Save("ListColumnRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
