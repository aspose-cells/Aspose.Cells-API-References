##Workbook.SaveToStream
Workbook method. Saves Excel file to a MemoryStream object as an Excel972003 xls file and returns it
## Workbook.SaveToStream method
Saves Excel file to a MemoryStream object as an Excel97-2003 xls file and returns it.
```csharp
public MemoryStream SaveToStream()
```
### Return Value
MemoryStream object which contains an xls Excel file.
### Remarks
This method provides same function as Save method and only save the workbook as Excel97-2003 xls file. It's mainly for calling from COM clients.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodSaveToStreamDemo
{
public static void Run()
{
// Create a new workbook
Workbook start = new Workbook();
// Access first worksheet and add some sample data
Worksheet worksheet = start.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
// Save workbook to memory stream
MemoryStream stream = start.SaveToStream();
// Create new workbook from the stream
Workbook workbook = new Workbook(stream);
// Modify the new workbook
Worksheet newWorksheet = workbook.Worksheets[0];
var area = CellArea.CreateCellArea(3, 0, 3, 1);
newWorksheet.Cells.InsertRange(area, 3, ShiftType.Down, true);
newWorksheet.Cells["A4"].PutValue("D");
newWorksheet.Cells["B4"].PutValue(40);
newWorksheet.Cells["A5"].PutValue("E");
newWorksheet.Cells["B5"].PutValue(50);
newWorksheet.Cells["A6"].PutValue("F");
newWorksheet.Cells["B6"].PutValue(60);
// Save the modified workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
