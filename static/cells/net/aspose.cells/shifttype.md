##Enum ShiftType
Aspose.Cells.ShiftType enum. Represent the shift options when deleting a range of cells
## ShiftType enumeration
Represent the shift options when deleting a range of cells.
```csharp
public enum ShiftType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Down | `0` | Shift cells down. |
| Left | `1` | Shift cells left. |
| None | `2` | Do not shift cells. |
| Right | `3` | Shift cells right. |
| Up | `4` | Shift cells up. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ShiftTypeDemo
{
public static void ShiftTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Cherry");
// Insert a new row at index 1, shifting existing rows down
worksheet.Cells.InsertRows(1, 1, true);
// Set a value in the newly inserted row
worksheet.Cells["A1"].PutValue("New Item");
// Delete a range of cells and shift cells up
worksheet.Cells.DeleteRange(2, 0, 2, 1, ShiftType.Up);
// Output the remaining values in the first column
for (int row = 0; row < worksheet.Cells.MaxDataRow + 1; row++)
{
Console.WriteLine(worksheet.Cells[row, 0].StringValue);
}
// Save the workbook
workbook.Save("ShiftTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
