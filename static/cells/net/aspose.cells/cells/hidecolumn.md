##Cells.HideColumn
Cells method. Hides a column
## Cells.HideColumn method
Hides a column.
```csharp
public void HideColumn(int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodHideColumnWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set some data in the column we'll hide
cells["B1"].PutValue("This column will be hidden");
cells["B2"].PutValue(123.45);
// Hide column B (index 1)
cells.HideColumn(1);
// Unhide the column with standard width
cells.UnhideColumn(1, cells.StandardWidth);
// Save the workbook
workbook.Save("HideColumnDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
