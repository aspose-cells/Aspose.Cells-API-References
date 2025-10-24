##DataSorter.Order1
DataSorter property. Represents sort order of the first key
## DataSorter.Order1 property
Represents sort order of the first key.
```csharp
public SortOrder Order1 { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterPropertyOrder1Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Score");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(85);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(92);
worksheet.Cells["A4"].PutValue("Bob");
worksheet.Cells["B4"].PutValue(78);
// Set data sorter properties
DataSorter sorter = workbook.DataSorter;
sorter.Order1 = SortOrder.Ascending;
sorter.Key1 = 1; // Sort by column B (Score)
// Define sort range
CellArea area = CellArea.CreateCellArea("A1", "B4");
// Perform the sort
sorter.Sort(worksheet.Cells, area);
// Save the workbook
workbook.Save("SortedOutput.xlsx");
}
}
}
```
### See Also
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
