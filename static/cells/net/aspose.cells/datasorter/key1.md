##DataSorter.Key1
DataSorter property. Represents first sorted column indexabsolute position column A is 0 B is 1
## DataSorter.Key1 property
Represents first sorted column index(absolute position, column A is 0, B is 1, ...).
```csharp
public int Key1 { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterPropertyKey1Demo
{
public static void Run()
{
// Create a workbook and add sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].PutValue("Name");
cells["B1"].PutValue("Score");
cells["A2"].PutValue("John");
cells["B2"].PutValue(85);
cells["A3"].PutValue("Alice");
cells["B3"].PutValue(92);
cells["A4"].PutValue("Bob");
cells["B4"].PutValue(78);
// Create data sorter and set Key1 to sort by Score column (column B)
DataSorter sorter = workbook.DataSorter;
sorter.Key1 = 1; // Column index 1 (B)
sorter.Order1 = SortOrder.Descending;
// Define sort area (rows 1-4, all data columns)
CellArea sortArea = new CellArea();
sortArea.StartRow = 1;
sortArea.EndRow = 4;
sortArea.StartColumn = 0;
sortArea.EndColumn = cells.MaxDataColumn;
// Perform the sort
sorter.Sort(cells, sortArea);
// Save the result
workbook.Save("SortedData.xlsx");
}
}
}
```
### See Also
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
