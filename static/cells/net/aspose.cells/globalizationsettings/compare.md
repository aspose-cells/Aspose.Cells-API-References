##GlobalizationSettings.Compare
GlobalizationSettings method. Compares two string values according to certain collation rules
## GlobalizationSettings.Compare method
Compares two string values according to certain collation rules.
```csharp
public virtual int Compare(string v1, string v2, bool ignoreCase)
```
| Parameter | Type | Description |
| --- | --- | --- |
| v1 | String | the first string |
| v2 | String | the second string |
| ignoreCase | Boolean | whether ignore case when comparing values |
### Return Value
Integer that indicates the lexical relationship between the two comparands
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class GlobalizationSettingsMethodCompareWithStringStringBooleanDemo
{
public static void Run()
{
// Create workbook with custom globalization settings
Workbook workbook = new Workbook();
workbook.Settings.GlobalizationSettings = new CustomComparisonSettings();
try
{
// Demonstrate direct Compare method usage
GlobalizationSettings settings = workbook.Settings.GlobalizationSettings;
int result1 = settings.Compare("Apple", "apple", true);
int result2 = settings.Compare("Apple", "apple", false);
Console.WriteLine($"Case-insensitive comparison result: {result1}");
Console.WriteLine($"Case-sensitive comparison result: {result2}");
// Demonstrate effect on spreadsheet operations
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Banana");
worksheet.Cells["A2"].PutValue("apple");
worksheet.Cells["A3"].PutValue("Cherry");
// Sort data using custom comparison
DataSorter sorter = workbook.DataSorter;
sorter.Order1 = SortOrder.Ascending;
sorter.Key1 = 0;
sorter.Sort(worksheet.Cells, 0, 0, 2, 0); // Corrected range to rows 0-2
Console.WriteLine("Sorted data with custom comparison rules:");
for (int row = 0; row < 3; row++)
{
Cell cell = worksheet.Cells[row, 0];
Console.WriteLine(cell.StringValue);
}
workbook.Save("GlobalizationCompareDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
public class CustomComparisonSettings : GlobalizationSettings
{
public override int Compare(string v1, string v2, bool ignoreCase)
{
// Implement custom comparison logic
var comparison = ignoreCase ?
StringComparison.OrdinalIgnoreCase :
StringComparison.Ordinal;
return string.Compare(v1?.Trim() ?? "", v2?.Trim() ?? "", comparison);
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
