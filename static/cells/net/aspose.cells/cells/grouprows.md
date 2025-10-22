##Cells.GroupRows
Cells method. Groups rows
## GroupRows(int, int, bool) {#grouprows_1}
Groups rows.
```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be grouped. |
| lastIndex | Int32 | The last row index to be grouped. |
| isHidden | Boolean | Specifies if the grouped rows are hidden. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGroupRowsWithInt32Int32BooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate some data
for (int i = 0; i < 10; i++)
{
cells[i, 0].PutValue($"Group {i + 1}");
for (int j = 1; j <= 5; j++)
{
cells[i, j].PutValue($"Data {j}");
}
}
// Group rows 1 to 5 (0-based index) and hide them
cells.GroupRows(1, 5, true);
// Set summary row below the group
worksheet.Outline.SummaryRowBelow = false;
// Save the workbook
workbook.Save("GroupRowsDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GroupRows(int, int) {#grouprows}
Groups rows.
```csharp
public void GroupRows(int firstIndex, int lastIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be grouped. |
| lastIndex | Int32 | The last row index to be grouped. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGroupRowsWithInt32Int32Demo
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
cells[i, 0].PutValue("Row " + (i + 1));
}
// Group rows 2 to 5 (zero-based index)
cells.GroupRows(1, 4);
// Save the workbook
workbook.Save("GroupRowsExample.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
