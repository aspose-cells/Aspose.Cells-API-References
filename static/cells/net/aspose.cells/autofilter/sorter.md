##AutoFilter.Sorter
AutoFilter property. Gets the data sorter
## AutoFilter.Sorter property
Gets the data sorter.
```csharp
public DataSorter Sorter { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterPropertySorterDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("C");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("A");
worksheet.Cells["B3"].PutValue(10);
worksheet.Cells["A4"].PutValue("B");
worksheet.Cells["B4"].PutValue(20);
// Create auto filter range
worksheet.AutoFilter.Range = "A1:B4";
// Get the auto filter
AutoFilter filter = worksheet.AutoFilter;
// Apply filter
filter.Filter(1, "10");
// Sort using the Sorter property
filter.Sorter.Sort();
// Save the workbook
workbook.Save("AutoFilterPropertySorterDemo.xlsx");
}
}
}
```
### See Also
* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
