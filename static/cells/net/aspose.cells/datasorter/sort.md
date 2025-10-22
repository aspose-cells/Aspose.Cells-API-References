##DataSorter.Sort
DataSorter method. Sorts the data of the area
## Sort(Cells, int, int, int, int) {#sort_2}
Sorts the data of the area.
```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| startRow | Int32 | The start row of the area. |
| startColumn | Int32 | The start column of the area. |
| endRow | Int32 | The end row of the area. |
| endColumn | Int32 | The end column of the area. |
### Return Value
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterMethodSortWithCellsInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Populate sample data
for (int i = 0; i < 6; i++)
{
cells[i, 0].PutValue(6 - i);
}
// Hide a row to demonstrate sorting with hidden rows
cells.Rows[1].IsHidden = true;
// Create and configure sorter
DataSorter sorter = wb.DataSorter;
sorter.AddKey(0, SortOrder.Ascending);
// Demonstrate Sort method with Cells and Int32 parameters
sorter.Sort(cells, 0, 0, 5, 0);
// Output results to console
for (int i = 0; i < 6; i++)
{
Console.WriteLine($"Cell A{i+1}: {cells[i, 0].IntValue}");
}
Console.WriteLine($"Is row 2 hidden? {cells.Rows[1].IsHidden}");
}
}
}
```
### See Also
* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Sort(Cells, CellArea) {#sort_1}
Sort the data of the area.
```csharp
public int[] Sort(Cells cells, CellArea area)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| area | CellArea | The area needed to sort |
### Return Value
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterMethodSortWithCellsCellAreaDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Year");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue(1995);
worksheet.Cells["B2"].PutValue(10000);
worksheet.Cells["A3"].PutValue(1996);
worksheet.Cells["B3"].PutValue(15000);
worksheet.Cells["A4"].PutValue(1997);
worksheet.Cells["B4"].PutValue(12000);
worksheet.Cells["A5"].PutValue(1998);
worksheet.Cells["B5"].PutValue(18000);
// Create data sorter
DataSorter dataSorter = workbook.DataSorter;
dataSorter.HasHeaders = true;
dataSorter.Key1 = 0; // Sort by first column (Year)
dataSorter.Order1 = SortOrder.Descending;
// Define sort area
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 4;
area.EndColumn = 1;
// Perform sort
dataSorter.Sort(worksheet.Cells, area);
// Save the workbook
workbook.Save("SortedData.xlsx");
}
}
}
```
### See Also
* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Sort() {#sort}
Sort the data in the range.
```csharp
public int[] Sort()
```
### Return Value
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterMethodSortDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to sort
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("C");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("A");
worksheet.Cells["B3"].PutValue(10);
worksheet.Cells["A4"].PutValue("B");
worksheet.Cells["B4"].PutValue(20);
// Create a table/list object
int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
table.ShowTotals = true;
// Sort the data by the first column
table.AutoFilter.Sorter.Sort();
// Save the workbook
workbook.Save("SortedData.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
