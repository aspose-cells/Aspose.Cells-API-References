##AutoFilter.SetRange
AutoFilter method. Sets the range to which the specified AutoFilter applies
## AutoFilter.SetRange method
Sets the range to which the specified AutoFilter applies.
```csharp
public void SetRange(int row, int startColumn, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| startColumn | Int32 | Start column index. |
| endColumn | Int32 | End column Index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodSetRangeWithInt32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Header");
sheet.Cells["A2"].PutValue("Data1");
sheet.Cells["A3"].PutValue("Data2");
sheet.Cells["A4"].PutValue("Data3");
// Set auto filter range (firstRow, firstColumn, totalRows)
sheet.AutoFilter.SetRange(0, 0, 4);
// Apply filter
sheet.AutoFilter.Custom(0, FilterOperatorType.Equal, "Data2");
// Refresh filter
sheet.AutoFilter.Refresh();
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
