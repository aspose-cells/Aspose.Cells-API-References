##DynamicFilter.Value
DynamicFilter property. Gets and sets the dynamic filter value
## DynamicFilter.Value property
Gets and sets the dynamic filter value.
```csharp
public object Value { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DynamicFilterPropertyValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));
// Create auto filter
worksheet.AutoFilter.Range = "A1:A5";
worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;
// Display current filter value
Console.WriteLine("Current DynamicFilter Value: " + filter.Value);
// Change the filter value to show April dates
filter.Value = new DateTime(2023, 4, 1);
filter.DynamicFilterType = DynamicFilterType.April;
// Apply the filter
worksheet.AutoFilter.Refresh();
// Save the result
workbook.Save("DynamicFilterValueDemo.xlsx");
}
}
}
```
### See Also
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
