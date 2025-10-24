##DataSorter.Key3
DataSorter property. Represents third sorted column indexabsolute position column A is 0 B is 1
## DataSorter.Key3 property
Represents third sorted column index(absolute position, column A is 0, B is 1, ...).
```csharp
public int Key3 { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterPropertyKey3Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].PutValue("Name");
cells["B1"].PutValue("Score");
cells["C1"].PutValue("Grade");
cells["A2"].PutValue("John");
cells["B2"].PutValue(85);
cells["C2"].PutValue("B");
cells["A3"].PutValue("Alice");
cells["B3"].PutValue(92);
cells["C3"].PutValue("A");
cells["A4"].PutValue("Bob");
cells["B4"].PutValue(78);
cells["C4"].PutValue("C");
cells["A5"].PutValue("Eve");
cells["B5"].PutValue(92);
cells["C5"].PutValue("A");
// Create data sorter
DataSorter sorter = workbook.DataSorter;
// Sort by Score (descending), then by Name (ascending), then by Grade (descending)
sorter.Order1 = SortOrder.Descending;
sorter.Key1 = 1; // Column B (Score)
sorter.Order2 = SortOrder.Ascending;
sorter.Key2 = 0; // Column A (Name)
sorter.Order3 = SortOrder.Descending;
sorter.Key3 = 2; // Column C (Grade)
// Sort data range
sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 5, 2));
// Save the workbook
workbook.Save("SortedData.xlsx");
}
}
}
```
### See Also
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
