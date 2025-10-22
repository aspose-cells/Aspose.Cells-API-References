##FilterColumnCollection.Item
FilterColumnCollection property. Gets FilterColumn object at the special field
## FilterColumnCollection indexer
Gets [`FilterColumn`](../../filtercolumn/) object at the special field.
```csharp
public FilterColumn this[int fieldIndex] { get; }
```
| Parameter | Description |
| --- | --- |
| fieldIndex | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
### Return Value
Returns [`FilterColumn`](../../filtercolumn/) object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FilterColumnCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Header");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["A3"].PutValue("Banana");
sheet.Cells["A4"].PutValue("Cherry");
sheet.Cells["A5"].PutValue("Date");
// Apply auto filter
sheet.AutoFilter.Range = "A1:A5";
sheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "e");
// Access filter using Item property
AutoFilter filter = sheet.AutoFilter;
FilterColumn filterColumn = filter.FilterColumns[0]; // Using Item property
CustomFilterCollection customFilters = (CustomFilterCollection)filterColumn.Filter;
CustomFilter firstFilter = customFilters[0];
// Display filter properties
Console.WriteLine("Filter Operator Type: " + firstFilter.FilterOperatorType);
Console.WriteLine("Filter Criteria: " + firstFilter.Criteria);
// Modify filter
firstFilter.FilterOperatorType = FilterOperatorType.EndsWith;
Console.WriteLine("\nModified Filter Operator Type: " + firstFilter.FilterOperatorType);
// Save the workbook
wb.Save("FilterExample.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
