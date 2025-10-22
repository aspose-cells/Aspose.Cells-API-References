##Worksheet.FreezePanes
Worksheet method. Freezes panes at the specified cell in the worksheet
## FreezePanes(int, int, int, int) {#freezepanes}
Freezes panes at the specified cell in the worksheet.
```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| column | Int32 | Column index. |
| freezedRows | Int32 | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Int32 | Number of visible columns in left pane, no more than column index. |
### Remarks
Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.
The first two parameters specify the froze position and the last two parameters specify the area frozen on the left top pane.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodFreezePanesWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Freeze panes at row 3, column 3, with 3 frozen rows and 3 frozen columns
worksheet.FreezePanes(3, 3, 3, 3);
// Save the workbook
workbook.Save("FreezePanesDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## FreezePanes(string, int, int) {#freezepanes_1}
Freezes panes at the specified cell in the worksheet.
```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| freezedRows | Int32 | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Int32 | Number of visible columns in left pane, no more than column index. |
### Remarks
Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodFreezePanesWithStringInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Freeze panes at "C3" with 3 frozen rows and 3 frozen columns
worksheet.FreezePanes("C3", 3, 3);
// Save the workbook
workbook.Save("FreezePanesDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
