##ListObject.EndRow
ListObject property. Gets the end row of the range
## ListObject.EndRow property
Gets the end row of the range.
```csharp
public int EndRow { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyEndRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Create sample data
sheet.Cells["A1"].PutValue("Name");
sheet.Cells["B1"].PutValue("Age");
sheet.Cells["A2"].PutValue("John");
sheet.Cells["B2"].PutValue(30);
sheet.Cells["A3"].PutValue("Mary");
sheet.Cells["B3"].PutValue(25);
// Create list object/table
int idx = sheet.ListObjects.Add(0, 0, 3, 1, true);
ListObject table = sheet.ListObjects[idx];
// Display initial EndRow
Console.WriteLine("Initial EndRow: " + table.EndRow);
// Add new row to the table
table.PutCellValue(4, 0, "Tom");
table.PutCellValue(4, 1, 28);
// Display updated EndRow
Console.WriteLine("Updated EndRow: " + table.EndRow);
// Save the workbook
wb.Save("ListObjectEndRowDemo.xlsx");
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
