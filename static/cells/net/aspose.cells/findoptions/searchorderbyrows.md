##FindOptions.SearchOrderByRows
FindOptions property. Indicates whether search order by rows or columns
## FindOptions.SearchOrderByRows property
Indicates whether search order by rows or columns.
```csharp
public bool SearchOrderByRows { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsPropertySearchOrderByRowsDemo
{
public static void Run()
{
// Create a workbook and add sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate cells with test data (searching for "abc" in column-major order)
worksheet.Cells["A1"].PutValue("xyz");
worksheet.Cells["B1"].PutValue("def");
worksheet.Cells["A2"].PutValue("123");
worksheet.Cells["B2"].PutValue("abc");
worksheet.Cells["A3"].PutValue("abc");
worksheet.Cells["B3"].PutValue("789");
// Create find options and set search order to column-major
FindOptions findOptions = new FindOptions();
findOptions.SearchOrderByRows = false; // Search column by column
// Find "abc" - should return A3 (row 2, column 0) when searching column-major
Cell foundCell = worksheet.Cells.Find("abc", null, findOptions);
// Output the result
Console.WriteLine($"Found 'abc' at row: {foundCell.Row}, column: {foundCell.Column}");
}
}
}
```
### See Also
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
