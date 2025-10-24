##Worksheet.GetAdvancedFilter
Worksheet method. Gets the settings of advanced filter
## Worksheet.GetAdvancedFilter method
Gets the settings of advanced filter.
```csharp
public AdvancedFilter GetAdvancedFilter()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodGetAdvancedFilterDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Setup data for filtering
sheet.Cells["A1"].PutValue("Name");
sheet.Cells["A2"].PutValue("John");
sheet.Cells["A3"].PutValue("Alice");
sheet.Cells["A4"].PutValue("Bob");
// Setup criteria range
sheet.Cells["C1"].PutValue("Name");
sheet.Cells["C2"].PutValue("John");
// Apply advanced filter
sheet.AdvancedFilter(true, "A1:A4", "C1:C2", "E1", false);
// Get the advanced filter
AdvancedFilter filter = sheet.GetAdvancedFilter();
// Output filter ranges
Console.WriteLine("List Range: " + filter.ListRange);
Console.WriteLine("Criteria Range: " + filter.CriteriaRange);
Console.WriteLine("Copy To Range: " + filter.CopyToRange);
}
}
}
```
### See Also
* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
