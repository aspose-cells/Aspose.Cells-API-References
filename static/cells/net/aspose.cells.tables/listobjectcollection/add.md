##ListObjectCollection.Add
ListObjectCollection method. Adds a ListObject to the worksheet
## Add(int, int, int, int, bool) {#add}
Adds a ListObject to the worksheet.
```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row of the list range. |
| startColumn | Int32 | The start row of the list range. |
| endRow | Int32 | The start row of the list range. |
| endColumn | Int32 | The start row of the list range. |
| hasHeaders | Boolean | Whether the range has headers. |
### Return Value
The index of the new ListObject
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ListObjectCollectionMethodAddWithInt32Int32Int32Int32BooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate data in a range
var range = worksheet.Cells.CreateRange("B3:D4");
range.Value = new object[,]
{
{"Col1", "Col2", "Col3"},
{100, 200, 300}
};
// Add ListObject using Add method with Int32 parameters
int firstRow = range.FirstRow;
int firstColumn = range.FirstColumn;
int endRow = firstRow + range.RowCount - 1;
int endColumn = firstColumn + range.ColumnCount - 1;
worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);
// Enable totals and set formula for one column
worksheet.ListObjects[0].ShowTotals = true;
worksheet.Cells["D5"].Formula = "=SUBTOTAL(109,[Col3])";
// Save the workbook
workbook.Save("ListObjectAddDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
## Add(string, string, bool) {#add_1}
Adds a ListObject to the worksheet.
```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startCell | String | The start cell of the list range. |
| endCell | String | The end cell of the list range. |
| hasHeaders | Boolean | Whether the range has headers. |
### Return Value
The index of the new ListObject
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectCollectionMethodAddWithStringStringBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue(2);
worksheet.Cells["A3"].PutValue(3);
worksheet.Cells["B3"].PutValue(4);
// Add list object using string range references
ListObjectCollection listObjects = worksheet.ListObjects;
listObjects.Add("A1", "B3", true);
workbook.Save("ListObjectExample.xlsx");
}
}
}
```
### See Also
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
