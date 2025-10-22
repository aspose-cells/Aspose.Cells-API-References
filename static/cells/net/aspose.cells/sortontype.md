##Enum SortOnType
Aspose.Cells.SortOnType enum. Sorted value type
## SortOnType enumeration
Sorted value type.
```csharp
public enum SortOnType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Value | `0` | Sorts by cells' value. |
| CellColor | `1` | Sorts by cells' color. |
| FontColor | `2` | Sorts by cells' font color. |
| Icon | `3` | Sorts by conditional icon. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SortOnTypeDemo
{
public static void SortOnTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["A4"].PutValue("Doe");
worksheet.Cells["B1"].PutValue("Score");
worksheet.Cells["B2"].PutValue(85);
worksheet.Cells["B3"].PutValue(95);
worksheet.Cells["B4"].PutValue(75);
// Apply auto filter to the range
worksheet.AutoFilter.Range = "A1:B4";
// Get the auto filter
AutoFilter autoFilter = worksheet.AutoFilter;
// Get the data sorter
DataSorter sorter = autoFilter.Sorter;
// Set the first key to sort by the values in the second column (Score)
sorter.AddKey(1, SortOnType.Value, SortOrder.Descending, null);
// Sort the data in the range
sorter.Sort(worksheet.Cells, 1, 0, 3, 1);
// Save the workbook
workbook.Save("SortOnTypeExample.xlsx");
// Output the results
Console.WriteLine("Data sorted by Score in descending order.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
