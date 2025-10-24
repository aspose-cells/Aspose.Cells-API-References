##Cells.DeleteColumns
Cells method. Deletes several columns
## DeleteColumns(int, int, bool) {#deletecolumns_1}
Deletes several columns.
```csharp
public void DeleteColumns(int columnIndex, int totalColumns, bool updateReference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the first column to be deleted. |
| totalColumns | Int32 | Count of columns to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteColumnsWithInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Column 1");
worksheet.Cells["B1"].PutValue("Column 2");
worksheet.Cells["C1"].PutValue("Column 3");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["B2"].PutValue(200);
worksheet.Cells["C2"].PutValue(300);
// Add a formula that references these columns
worksheet.Cells["D1"].Formula = "=SUM(A2:C2)";
Console.WriteLine("Before deleting columns:");
Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
Console.WriteLine("C1: " + worksheet.Cells["C1"].Value);
Console.WriteLine("D1 formula: " + worksheet.Cells["D1"].Formula);
// Delete column B (index 1) and shift remaining columns left
worksheet.Cells.DeleteColumns(1, 1, true);
Console.WriteLine("\nAfter deleting column B:");
Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
Console.WriteLine("C1 formula: " + worksheet.Cells["C1"].Formula);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## DeleteColumns(int, int, DeleteOptions) {#deletecolumns}
Deletes several columns.
```csharp
public void DeleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the first column to be deleted. |
| totalColumns | Int32 | Count of columns to be deleted. |
| options | DeleteOptions | Options for the deleting operation |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodDeleteColumnsWithInt32Int32DeleteOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data in columns A-E
for (int col = 0; col < 5; col++)
{
worksheet.Cells[0, col].Value = $"Column {(char)('A' + col)}";
worksheet.Cells[1, col].Value = $"Data{col + 1}";
}
// Create DeleteOptions and configure settings
DeleteOptions options = new DeleteOptions
{
UpdateReference = true // Update references in other cells
};
try
{
// Delete 2 columns starting from column B (index 1)
worksheet.Cells.DeleteColumns(1, 2, options);
Console.WriteLine("Deleted columns B and C successfully");
// Display remaining data in column B (original column D)
Console.WriteLine($"New column B value: {worksheet.Cells[1, 1].StringValue}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing DeleteColumns: {ex.Message}");
}
// Save the modified workbook
workbook.Save("DeleteColumnsWithOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
