##Worksheet.MoveTo
Worksheet method. Moves the sheet to another location in the spreadsheet
## Worksheet.MoveTo method
Moves the sheet to another location in the spreadsheet.
```csharp
public void MoveTo(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | Destination sheet index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodMoveToWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some worksheets
workbook.Worksheets.Add("Sheet1");
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Add a new worksheet and move it to position 1
Worksheet newWorksheet = workbook.Worksheets.Add("MovedSheet");
newWorksheet.MoveTo(1);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
