##ListObject.DataRange
ListObject property. Gets the data range of the ListObject
## ListObject.DataRange property
Gets the data range of the ListObject.
```csharp
public Range DataRange { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ListObjectPropertyDataRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Mary");
// Create a ListObject (Table)
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];
table.DisplayName = "EmployeeTable";
// Get the data range of the table
Aspose.Cells.Range dataRange = table.DataRange;
// Demonstrate DataRange usage
Console.WriteLine("Table Data Range: " + dataRange.Address);
Console.WriteLine("Row Count: " + dataRange.RowCount);
Console.WriteLine("Column Count: " + dataRange.ColumnCount);
// Add a formula to the last column using DataRange
string formula = "=CONCATENATE(\"ID-\", [ID])";
int lastColIndex = dataRange.ColumnCount;
dataRange[0, lastColIndex].PutValue("FormattedID");
for (int i = 1; i < dataRange.RowCount; i++)
{
dataRange[i, lastColIndex].Formula = formula;
}
// Save the workbook
workbook.Save("ListObjectDataRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../../../aspose.cells/range/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
