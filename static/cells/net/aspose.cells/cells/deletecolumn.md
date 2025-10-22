##Cells.DeleteColumn
Cells method. Deletes a column
## DeleteColumn(int, bool) {#deletecolumn_1}
Deletes a column.
```csharp
public void DeleteColumn(int columnIndex, bool updateReference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the column to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteColumnWithInt32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Fill some sample data into cells
for (int i = 0; i < 5; i++)
{
for (int j = 0; j < 5; j++)
{
sheet.Cells[i, j].PutValue($"Data {i},{j}");
}
}
Console.WriteLine("Before deleting column:");
PrintCellValues(sheet);
// Delete the first column and shift remaining columns left
sheet.Cells.DeleteColumn(0, true);
Console.WriteLine("\nAfter deleting column 0:");
PrintCellValues(sheet);
// Save the workbook
workbook.Save("DeleteColumnDemo.xlsx");
}
private static void PrintCellValues(Worksheet sheet)
{
for (int i = 0; i < 5; i++)
{
for (int j = 0; j < 5; j++)
{
Console.Write(sheet.Cells[i, j].Value + "\t");
}
Console.WriteLine();
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## DeleteColumn(int) {#deletecolumn}
Deletes a column.
```csharp
public void DeleteColumn(int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the column to be deleted. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteColumnWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Fill some sample data in columns
Cells cells = sheet.Cells;
cells["A1"].PutValue("Column A");
cells["B1"].PutValue("Column B");
cells["C1"].PutValue("Column C");
// Delete column at index 1 (Column B)
cells.DeleteColumn(1);
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("Column deleted successfully.");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
