##ListObject.Resize
ListObject method. Resize the range of the list object
## ListObject.Resize method
Resize the range of the list object.
```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row index of the new range. |
| startColumn | Int32 | The start column index of the new range. |
| endRow | Int32 | The end row index of the new range. |
| endColumn | Int32 | The end column index of the new range. |
| hasHeaders | Boolean | Whether this table has headers. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectMethodResizeWithInt32Int32Int32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].PutValue("Item " + (i + 1));
worksheet.Cells[i, 1].PutValue(i * 10);
}
// Create a list object
int index = worksheet.ListObjects.Add(0, 0, 5, 1, true);
ListObject listObj = worksheet.ListObjects[index];
listObj.TableStyleType = TableStyleType.TableStyleLight2;
// Resize the list object
listObj.Resize(0, 0, 9, 1, true);
// Save the workbook
workbook.Save("ResizedListObject.xlsx");
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
