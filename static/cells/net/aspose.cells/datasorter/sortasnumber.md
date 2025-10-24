##DataSorter.SortAsNumber
DataSorter property. Indicates whether sorting anything that looks like a number
## DataSorter.SortAsNumber property
Indicates whether sorting anything that looks like a number.
```csharp
public bool SortAsNumber { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterPropertySortAsNumberDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with mixed numbers and text numbers
worksheet.Cells["A1"].PutValue("Number");
worksheet.Cells["A2"].PutValue("2");
worksheet.Cells["A3"].PutValue("10");
worksheet.Cells["A4"].PutValue("1");
// Create cell area to sort
CellArea ca = CellArea.CreateCellArea("A1", "A4");
// Create data sorter
DataSorter sorter = workbook.DataSorter;
int idx = CellsHelper.ColumnNameToIndex("A");
// Add sort key (column A)
sorter.AddKey(idx, SortOrder.Ascending);
// Sort as numbers (true) or strings (false)
sorter.SortAsNumber = true;
sorter.Sort(worksheet.Cells, ca);
Console.WriteLine("Sorted as numbers:");
for (int i = 1; i <= 4; i++)
{
Console.WriteLine(worksheet.Cells["A" + i].StringValue);
}
// Reset data for second sort
worksheet.Cells["A2"].PutValue("2");
worksheet.Cells["A3"].PutValue("10");
worksheet.Cells["A4"].PutValue("1");
// Sort as strings
sorter.SortAsNumber = false;
sorter.Sort(worksheet.Cells, ca);
Console.WriteLine("\nSorted as strings:");
for (int i = 1; i <= 4; i++)
{
Console.WriteLine(worksheet.Cells["A" + i].StringValue);
}
}
}
}
```
### See Also
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
