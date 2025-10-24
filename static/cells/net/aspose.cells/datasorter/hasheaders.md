##DataSorter.HasHeaders
DataSorter property. Represents whether the range has headers
## DataSorter.HasHeaders property
Represents whether the range has headers.
```csharp
public bool HasHeaders { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterPropertyHasHeadersDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add headers and sample data
worksheet.Cells["A1"].PutValue("Fruits");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B2"].PutValue(15);
worksheet.Cells["B3"].PutValue(8);
worksheet.Cells["B4"].PutValue(12);
// Create data sorter and set HasHeaders to true
DataSorter sorter = workbook.DataSorter;
sorter.HasHeaders = true; // This tells the sorter the first row contains headers
// Sort by the first column (Fruits) in ascending order
sorter.AddKey(0, SortOrder.Ascending);
// Sort the data range (including headers)
sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "B4"));
// Save the sorted workbook
workbook.Save("SortedWithHeaders.xlsx");
}
}
}
```
### See Also
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
