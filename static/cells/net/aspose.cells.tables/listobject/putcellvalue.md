##ListObject.PutCellValue
ListObject method. Put the value to the cell
## PutCellValue(int, int, object) {#putcellvalue}
Put the value to the cell.
```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| value | Object | The cell value. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectMethodPutCellValueWithInt32Int32ObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
worksheet.Cells["A1"].PutValue("Column1");
worksheet.Cells["B1"].PutValue("Column2");
worksheet.Cells["C1"].PutValue("Column3");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["B2"].PutValue(200);
worksheet.Cells["C2"].PutValue(300);
// Create a list object
int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
ListObject listObject = worksheet.ListObjects[index];
// Demonstrate PutCellValue with Int32, Int32, Object parameters
listObject.PutCellValue(1, 0, 500); // Update row 1, column 0 with value 500
listObject.PutCellValue(1, 1, "Updated Value"); // Update row 1, column 1 with string
listObject.PutCellValue(1, 2, DateTime.Now); // Update row 1, column 2 with current date
// Save the workbook
workbook.Save("ListObjectPutCellValueDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
## PutCellValue(int, int, object, bool) {#putcellvalue_1}
Put the value to the cell.
```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value, bool isTotalsRowLabel)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| value | Object | The cell value. |
| isTotalsRowLabel | Boolean | Indicates whether it is a label for total row,only works for total row. If False and this row is total row, a new row will be inserted. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectMethodPutCellValueWithInt32Int32ObjectBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a ListObject
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Mary");
// Create a ListObject
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject listObject = worksheet.ListObjects[index];
// Use PutCellValue to update a cell (row 2, column 1) with new value and expand table
listObject.PutCellValue(2, 1, "Updated Value", true);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
