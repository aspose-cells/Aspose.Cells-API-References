##DataSorter.Key2
DataSorter property. Represents second sorted column indexabsolute position column A is 0 B is 1
## DataSorter.Key2 property
Represents second sorted column index(absolute position, column A is 0, B is 1, ...).
```csharp
public int Key2 { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterPropertyKey2Demo
{
public static void Run()
{
// Create a workbook and add sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
worksheet.Cells["A4"].PutValue("Bob");
worksheet.Cells["B4"].PutValue(35);
// Create DataSorter and set properties
DataSorter sorter = workbook.DataSorter;
sorter.HasHeaders = true;
sorter.Key1 = 0; // Sort by first column (Name)
sorter.Order1 = SortOrder.Ascending;
sorter.Key2 = 1; // Then sort by second column (Age)
sorter.Order2 = SortOrder.Descending;
// Sort data range
sorter.Sort(worksheet.Cells, 0, 0, 3, 1);
// Output the sorted data to demonstrate Key2 usage
Console.WriteLine("Sorted Data:");
for (int i = 0; i <= 3; i++)
{
Console.WriteLine($"{worksheet.Cells[i, 0].StringValue} - {worksheet.Cells[i, 1].IntValue}");
}
}
}
}
```
### See Also
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
