##Cells.HideRow
Cells method. Hides a row
## Cells.HideRow method
Hides a row.
```csharp
public void HideRow(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodHideRowWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Hide row 5
worksheet.Cells.HideRow(5);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
