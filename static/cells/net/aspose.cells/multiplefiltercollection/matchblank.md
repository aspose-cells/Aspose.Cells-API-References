##MultipleFilterCollection.MatchBlank
MultipleFilterCollection property. Indicates whether to filter by blank
## MultipleFilterCollection.MatchBlank property
Indicates whether to filter by blank.
```csharp
public bool MatchBlank { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MultipleFilterCollectionPropertyMatchBlankDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with some blank cells
worksheet.Cells["A1"].PutValue("Column1");
worksheet.Cells["A2"].PutValue("Value1");
worksheet.Cells["A3"].PutValue("");
worksheet.Cells["A4"].PutValue("Value2");
worksheet.Cells["A5"].PutValue(null);
// Apply auto filter
worksheet.AutoFilter.Range = "A1:A5";
AutoFilter filter = worksheet.AutoFilter;
// Add filters including blank values
filter.AddFilter(0, null);
filter.AddFilter(0, "");
filter.Refresh();
// Get the filter collection and check MatchBlank property
MultipleFilterCollection multiFilters = (MultipleFilterCollection)filter.FilterColumns[0].Filter;
Console.WriteLine("MatchBlank property value: " + multiFilters.MatchBlank);
// Save the workbook
workbook.Save("MatchBlankDemo.xlsx");
}
}
}
```
### See Also
* class [MultipleFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
