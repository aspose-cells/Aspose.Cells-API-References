##DataSorter.SortLeftToRight
DataSorter property. True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false
## DataSorter.SortLeftToRight property
True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.
```csharp
public bool SortLeftToRight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterPropertySortLeftToRightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data (columns will be treated as rows when SortLeftToRight=true)
worksheet.Cells["A1"].PutValue(3);
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B1"].PutValue("C");
worksheet.Cells["B2"].PutValue("A");
worksheet.Cells["B3"].PutValue("B");
// Create data sorter and set to sort left to right
DataSorter sorter = workbook.DataSorter;
sorter.SortLeftToRight = true;
// Set sort key (column index becomes row index when sorting left-to-right)
sorter.Key1 = 0; // Sort by first "row" (originally column A)
// Define sort area (rows become columns when sorting left-to-right)
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 2;
area.StartColumn = 0;
area.EndColumn = 1;
// Perform the sort
sorter.Sort(worksheet.Cells, area);
// Save the result
workbook.Save("SortedLeftToRight.xlsx");
}
}
}
```
### See Also
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
