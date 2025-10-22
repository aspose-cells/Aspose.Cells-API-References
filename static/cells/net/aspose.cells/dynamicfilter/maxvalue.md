##DynamicFilter.MaxValue
DynamicFilter property. Gets and sets the dynamic filter max value
## DynamicFilter.MaxValue property
Gets and sets the dynamic filter max value.
```csharp
public object MaxValue { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DynamicFilterPropertyMaxValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample numeric data
worksheet.Cells["A1"].PutValue("Values");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["A4"].PutValue(30);
worksheet.Cells["A5"].PutValue(40);
worksheet.Cells["A6"].PutValue(50);
// Create auto filter
worksheet.AutoFilter.Range = "A1:A6";
// Apply dynamic filter with range criteria
worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);
DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;
// Display current MaxValue
Console.WriteLine("Current MaxValue: " + filter.MaxValue);
// Since DynamicFilterType.Between doesn't exist, we'll use a different approach
// For example, we can use a custom filter instead
worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, 20);
worksheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, 40);
// Apply the filter
worksheet.AutoFilter.Refresh();
// Save the result
workbook.Save("DynamicFilterMaxValueDemo.xlsx");
}
}
}
```
### See Also
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
