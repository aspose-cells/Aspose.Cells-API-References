##Cells.DeleteRow
Cells method. Deletes a row
## DeleteRow(int) {#deleterow}
Deletes a row.
```csharp
public void DeleteRow(int rowIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index of the row to be deleted. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteRowWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Set a shared formula in row 66
cells[65, 0].SetSharedFormula("=SUM(B10:B66)", 1, 6);
// Delete row 9 (which will shift rows up)
cells.DeleteRow(9);
// Verify the formula was adjusted after row deletion
for (int i = 1; i < 7; i++)
{
char columnName = (char)('A' + i);
Console.WriteLine($"Cell {columnName}66 formula after deletion: {cells[64, i].Formula}");
}
// Delete rows 60-61 (which will shift rows up)
cells.DeleteRows(59, 2);
// Verify the formula was adjusted after rows deletion
for (int i = 1; i < 7; i++)
{
char columnName = (char)('A' + i);
Console.WriteLine($"Cell {columnName}64 formula after deletion: {cells[62, i].Formula}");
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## DeleteRow(int, bool) {#deleterow_1}
Deletes a row.
```csharp
public void DeleteRow(int rowIndex, bool updateReference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index of the row to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteRowWithInt32BooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Item");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["A3"].PutValue("Banana");
sheet.Cells["A4"].PutValue("Cherry");
Console.WriteLine("Original Data:");
for (int i = 1; i <= 4; i++)
{
Console.WriteLine(sheet.Cells[$"A{i}"].Value);
}
sheet.Cells.DeleteRow(2, true);
Console.WriteLine("\nData After Deletion:");
for (int i = 1; i <= 3; i++)
{
Console.WriteLine(sheet.Cells[$"A{i}"].Value);
}
workbook.Save("DeleteRowExample.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
