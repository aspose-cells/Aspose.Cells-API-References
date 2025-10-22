##Cells.InsertRow
Cells method. Inserts a new row into the worksheet
## Cells.InsertRow method
Inserts a new row into the worksheet.
```csharp
public void InsertRow(int rowIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertRowWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Get cells collection
Cells cells = sheet.Cells;
// Insert sample data in row 6
cells[6, 0].PutValue("Original Row 6");
cells[6, 1].PutValue(100);
// Insert sample data in row 7
cells[7, 0].PutValue("Original Row 7");
cells[7, 1].PutValue(200);
// Insert a new row at index 7 (pushes existing row 7 down)
cells.InsertRow(7);
// Add data to the newly inserted row
cells[7, 0].PutValue("New Inserted Row");
cells[7, 1].PutValue(150);
// Save the workbook
workbook.Save("InsertRowDemo.xlsx");
Console.WriteLine("Row inserted successfully at index 7.");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
