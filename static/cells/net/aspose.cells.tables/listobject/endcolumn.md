##ListObject.EndColumn
ListObject property. Gets the end column of the range
## ListObject.EndColumn property
Gets the end column of the range.
```csharp
public int EndColumn { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyEndColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["C1"].PutValue("Age");
for (int i = 2; i <= 5; i++)
{
worksheet.Cells[$"A{i}"].PutValue(i-1);
worksheet.Cells[$"B{i}"].PutValue($"Person {i-1}");
worksheet.Cells[$"C{i}"].PutValue(20 + i);
}
// Create a list object/table
int listObjectIndex = worksheet.ListObjects.Add(0, 0, 4, 2, true);
ListObject table = worksheet.ListObjects[listObjectIndex];
table.ShowTotals = true;
// Display original end column
Console.WriteLine($"Original EndColumn: {table.EndColumn}");
// Resize the table to include one more column
table.Resize(table.StartRow, table.StartColumn, table.EndRow, table.EndColumn + 1, table.ShowHeaderRow);
// Display new end column
Console.WriteLine($"New EndColumn: {table.EndColumn}");
// Save the workbook
workbook.Save("ListObjectEndColumnDemo.xlsx");
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
