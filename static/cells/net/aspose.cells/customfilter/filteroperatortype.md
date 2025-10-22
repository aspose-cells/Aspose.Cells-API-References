##CustomFilter.FilterOperatorType
CustomFilter property. Gets and sets the filter operator type
## CustomFilter.FilterOperatorType property
Gets and sets the filter operator type.
```csharp
public FilterOperatorType FilterOperatorType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomFilterPropertyFilterOperatorTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Names");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["A4"].PutValue("Mike");
worksheet.Cells["A5"].PutValue("Emily");
// Apply auto filter
worksheet.AutoFilter.Range = "A1:A5";
AutoFilter filter = worksheet.AutoFilter;
// Apply custom filter with Contains operator
filter.Custom(0, FilterOperatorType.Contains, "e");
// Get the first custom filter
CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
// Demonstrate FilterOperatorType property
Console.WriteLine("Initial Filter Operator: " + customFilter.FilterOperatorType);
Console.WriteLine("Criteria: " + customFilter.Criteria);
// Change the filter operator type
customFilter.FilterOperatorType = FilterOperatorType.EndsWith;
Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
// Save the workbook
workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
