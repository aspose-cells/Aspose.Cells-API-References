##AutoFilter.AddFilter
AutoFilter method. Adds a filter for a filter column
## AutoFilter.AddFilter method
Adds a filter for a filter column.
```csharp
public void AddFilter(int fieldIndex, string criteria)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |
### Remarks
MS Excel 2007 supports multiple selection in a filter column.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodAddFilterWithInt32StringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Fruits");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Cherry");
worksheet.Cells["A5"].PutValue("Date");
worksheet.Cells["A6"].PutValue("Elderberry");
// Create auto filter range
worksheet.AutoFilter.Range = "A1:A6";
// Get the auto filter
AutoFilter filter = worksheet.AutoFilter;
// Add filters for values starting with 'A' and 'E'
filter.AddFilter(0, "A*");
filter.AddFilter(0, "E*");
// Refresh the filter
filter.Refresh();
// Save the workbook
workbook.Save("AutoFilterAddFilterDemo.xlsx");
}
}
}
```
### See Also
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
