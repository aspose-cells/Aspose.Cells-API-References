##Cells.HideColumns
Cells method. Hide multiple columns
## Cells.HideColumns method
Hide multiple columns.
```csharp
public void HideColumns(int column, int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| totalColumns | Int32 | Column number. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodHideColumnsWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate some sample data
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 10; j++)
{
cells[i, j].PutValue($"Data {i},{j}");
}
}
// Hide columns 3 through 5 (zero-based index)
int startColumn = 2; // Column C
int columnCount = 3;  // Hide 3 columns
cells.HideColumns(startColumn, columnCount);
// Save the workbook
workbook.Save("HideColumnsDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
