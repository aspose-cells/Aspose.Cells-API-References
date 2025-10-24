##Cells.GroupColumns
Cells method. Groups columns
## GroupColumns(int, int) {#groupcolumns}
Groups columns.
```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first column index to be grouped. |
| lastIndex | Int32 | The last column index to be grouped. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGroupColumnsWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Group columns from index 0 to 255
cells.GroupColumns(0, 255);
// Save the workbook
string outputPath = "outputGroupColumns.xlsx";
workbook.Save(outputPath);
Console.WriteLine("Columns grouped successfully. File saved to: " + outputPath);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GroupColumns(int, int, bool) {#groupcolumns_1}
Groups columns.
```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first column index to be grouped. |
| lastIndex | Int32 | The last column index to be grouped. |
| isHidden | Boolean | Specifies if the grouped columns are hidden. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGroupColumnsWithInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Group columns 5 to 7 (3 columns) and hide them
cells.GroupColumns(5, 7, true);
// Save the workbook
workbook.Save("GroupColumnsOutput.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
