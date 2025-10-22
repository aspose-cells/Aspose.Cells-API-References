##Enum SortOrder
Aspose.Cells.SortOrder enum. Represents sort order for the data range
## SortOrder enumeration
Represents sort order for the data range.
```csharp
public enum SortOrder
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Ascending | `0` | Sorts data in ascending order |
| Descending | `1` | Sorts data in descending order |
| Natural | `2` | Keeps original data order without sorting. Only applies to some special scenarios such as PivotTable. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassSortOrderDemo
{
public static void Run()
{
// Create a new workbook
var workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to sort
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Score");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(85);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(92);
worksheet.Cells["A4"].PutValue("Bob");
worksheet.Cells["B4"].PutValue(78);
// Create data sorter
var sorter = workbook.DataSorter;
// Set sort order and keys
sorter.Order1 = SortOrder.Descending;
sorter.Key1 = 1; // Sort by column B (Score)
// Define sort area
var sortArea = new CellArea
{
StartRow = 0,
StartColumn = 0,
EndRow = 3,
EndColumn = 1
};
// Perform the sort
sorter.Sort(worksheet.Cells, sortArea);
// Save the workbook
workbook.Save("SortedData.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
