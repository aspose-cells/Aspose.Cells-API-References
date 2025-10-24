##AutoFilter.RemoveFilter
AutoFilter method. Removes a filter for a filter column
## RemoveFilter(int, string) {#removefilter_1}
Removes a filter for a filter column.
```csharp
public void RemoveFilter(int fieldIndex, string criteria)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AutoFilterMethodRemoveFilterWithInt32StringDemo
{
public static void Run()
{
// Create a new workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data for demonstration
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Category");
worksheet.Cells["C1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue("Electronics");
worksheet.Cells["C2"].PutValue(999.99);
worksheet.Cells["A3"].PutValue("Novel");
worksheet.Cells["B3"].PutValue("Books");
worksheet.Cells["C3"].PutValue(19.99);
worksheet.Cells["A4"].PutValue("Smartphone");
worksheet.Cells["B4"].PutValue("Electronics");
worksheet.Cells["C4"].PutValue(599.99);
// Set auto filter range (headers + 3 data rows)
worksheet.AutoFilter.SetRange(0, 0, 2);
try
{
AutoFilter autoFilter = worksheet.AutoFilter;
// Apply filter on Category column (fieldIndex 1) for "Electronics"
autoFilter.AddFilter(1, "Electronics");
autoFilter.Refresh(); // Apply filter to hide non-matching rows
// Remove the specific filter from Category column
autoFilter.RemoveFilter(1, "Electronics");
autoFilter.Refresh(); // Re-apply filter (now shows all rows)
Console.WriteLine("RemoveFilter executed: Electronics filter removed from Category column.");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
// Save the modified workbook
workbook.Save("AutoFilterMethodRemoveFilterWithInt32StringDemo.xlsx");
}
}
}
```
### See Also
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RemoveFilter(int) {#removefilter}
Remove the specific filter.
```csharp
public void RemoveFilter(int fieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The specific filter index |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodRemoveFilterWithInt32Demo
{
public static void Run()
{
// Create a workbook with sample data
Workbook wb = new Workbook();
Worksheet worksheet = wb.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Fruit");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["A5"].PutValue("Grape");
// Apply auto filter
worksheet.AutoFilter.Range = "A1:A5";
AutoFilter filter = worksheet.AutoFilter;
// Add a filter
filter.AddFilter(0, "Apple");
filter.Refresh();
Console.WriteLine("After adding filter - Visible rows:");
PrintVisibleRows(worksheet);
// Remove the filter
filter.RemoveFilter(0);
filter.Refresh();
Console.WriteLine("\nAfter removing filter - Visible rows:");
PrintVisibleRows(worksheet);
}
private static void PrintVisibleRows(Worksheet worksheet)
{
for (int i = 0; i < worksheet.Cells.MaxDataRow + 1; i++)
{
if (!worksheet.Cells.Rows[i].IsHidden)
{
Console.WriteLine($"Row {i + 1}: {worksheet.Cells[i, 0].StringValue}");
}
}
}
}
}
```
### See Also
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
