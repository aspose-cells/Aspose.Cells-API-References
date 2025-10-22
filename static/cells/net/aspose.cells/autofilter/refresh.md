##AutoFilter.Refresh
AutoFilter method. Refresh auto filters to hide or unhide the rows
## Refresh() {#refresh}
Refresh auto filters to hide or unhide the rows.
```csharp
public int[] Refresh()
```
### Return Value
Returns all hidden rows' indexes.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodRefreshDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["B6"].PutValue("Header1");
worksheet.Cells["C6"].PutValue("Header2");
worksheet.Cells["D6"].PutValue("Header3");
worksheet.Cells["E6"].PutValue("Values");
for (int i = 7; i <= 15; i++)
{
worksheet.Cells["B" + i].PutValue("Item " + (i-6));
worksheet.Cells["E" + i].PutValue((i-6) * 100);
}
// Apply auto filter
worksheet.AutoFilter.Range = "B6:E6";
// Filter values greater than 500
worksheet.AutoFilter.Custom(3, FilterOperatorType.GreaterThan, 500);
worksheet.AutoFilter.Refresh();
Console.WriteLine("Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
Console.WriteLine("Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
// Change filter to show values equal to 500 or greater than 700
worksheet.AutoFilter.Custom(3, FilterOperatorType.Equal, 500, false, FilterOperatorType.GreaterThan, 700);
worksheet.AutoFilter.Refresh();
Console.WriteLine("After refresh - Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
Console.WriteLine("After refresh - Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
}
}
}
```
### See Also
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Refresh(bool) {#refresh_1}
Gets all hidden rows' indexes.
```csharp
public int[] Refresh(bool hideRows)
```
| Parameter | Type | Description |
| --- | --- | --- |
| hideRows | Boolean | If true, hide the filtered rows. |
### Return Value
Returns all hidden rows indexes.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodRefreshWithBooleanDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Column1");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["A4"].PutValue(1);
worksheet.Cells["A5"].PutValue(3);
// Apply auto filter
worksheet.AutoFilter.Range = "A1:A5";
worksheet.AutoFilter.AddFilter(0, "1"); // Filter to show only rows with value 1
// Refresh the filter and get hidden rows
int[] hiddenRows = worksheet.AutoFilter.Refresh(false);
Console.WriteLine("Hidden rows after filter:");
if (hiddenRows != null)
{
foreach (int row in hiddenRows)
{
Console.WriteLine(row);
}
}
// Show all data and refresh again
worksheet.AutoFilter.ShowAll();
hiddenRows = worksheet.AutoFilter.Refresh(false);
Console.WriteLine("\nHidden rows after showing all:");
if (hiddenRows == null)
{
Console.WriteLine("No hidden rows");
}
}
}
}
```
### See Also
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
