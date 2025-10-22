##Cells.DeleteBlankRows
Cells method. Delete all blank rows which do not contain any data or other object
## DeleteBlankRows() {#deleteblankrows}
Delete all blank rows which do not contain any data or other object.
```csharp
public void DeleteBlankRows()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteBlankRowsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add some data with blank rows
cells["A1"].PutValue("Header");
cells["A2"].PutValue("Data1");
cells["A4"].PutValue("Data2"); // Blank row at A3
cells["A6"].PutValue("Data3"); // Blank row at A5
Console.WriteLine("Before deleting blank rows:");
for (int i = 0; i < 7; i++)
{
Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
}
// Delete blank rows
cells.DeleteBlankRows();
Console.WriteLine("\nAfter deleting blank rows:");
for (int i = 0; i < cells.MaxDataRow + 1; i++)
{
Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
}
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## DeleteBlankRows(DeleteOptions) {#deleteblankrows_1}
Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table.
```csharp
public void DeleteBlankRows(DeleteOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | DeleteOptions | The options of deleting range. |
### Remarks
For blank rows that will be deleted, it is not only required that [`IsBlank`](../../row/isblank/) should be true, but also there should be no visible comment defined for any cell in those rows, and no pivot table whose range intersects with them.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteBlankRowsWithDeleteOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add some test data with blank rows
sheet.Cells["A1"].PutValue("Data1");
sheet.Cells["A3"].PutValue("Data2");
sheet.Cells["A5"].PutValue("Data3");
// Create delete options
DeleteOptions options = new DeleteOptions();
options.UpdateReference = true;
// Delete blank rows
sheet.Cells.DeleteBlankRows(options);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
