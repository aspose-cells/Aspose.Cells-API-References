##Cells.DeleteBlankColumns
Cells method. Delete all blank columns which do not contain any data
## DeleteBlankColumns() {#deleteblankcolumns}
Delete all blank columns which do not contain any data.
```csharp
public void DeleteBlankColumns()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteBlankColumnsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some test data with blank columns
worksheet.Cells["A1"].PutValue("Column A");
worksheet.Cells["C1"].PutValue("Column C"); // Column B will be blank
worksheet.Cells["A2"].PutValue("Data A");
worksheet.Cells["C2"].PutValue("Data C");
// Delete blank columns
worksheet.Cells.DeleteBlankColumns();
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
## DeleteBlankColumns(DeleteOptions) {#deleteblankcolumns_1}
Delete all blank columns which do not contain any data.
```csharp
public void DeleteBlankColumns(DeleteOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | DeleteOptions | The options of deleting range. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteBlankColumnsWithDeleteOptionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data with blank columns
worksheet.Cells["A1"].PutValue("Column A");
worksheet.Cells["C1"].PutValue("Column C"); // Column B is blank
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["C2"].PutValue(3);
Console.WriteLine("Before deleting blank columns:");
Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 2 (0-based, column C)
// Set up delete options
DeleteOptions options = new DeleteOptions();
options.UpdateReference = true;
// Delete blank columns
worksheet.Cells.DeleteBlankColumns(options);
Console.WriteLine("After deleting blank columns:");
Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 1 (0-based, column A and C remain, B was deleted)
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
