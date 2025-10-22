##AbstractGlobalizationSettings.Compare
AbstractGlobalizationSettings method. Compares two string values according to certain collation rules
## AbstractGlobalizationSettings.Compare method
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
public class AbstractGlobalizationSettingsMethodCompareWithStringStringBooleanDemo
{
public static void Run()
{
// Create custom globalization settings that override the Compare method
var settings = new CustomGlobalizationSettings();
// Create a workbook with custom globalization settings
Workbook workbook = new Workbook();
workbook.Settings.GlobalizationSettings = settings;
// Prepare strings to compare
string string1 = "Apple";
string string2 = "apple";
bool ignoreCase = true;
try
{
// The Compare method will be called internally during operations like sorting
// We demonstrate direct usage here
int comparisonResult = settings.Compare(string1, string2, ignoreCase);
Console.WriteLine($"Comparison result: {comparisonResult}");
Console.WriteLine($"Strings compared: '{string1}' and '{string2}' (Ignore case: {ignoreCase})");
// Demonstrate effect by sorting data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Orange");
worksheet.Cells["A2"].PutValue("apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Apple");
// Create a DataSorter and set the range for sorting
DataSorter sorter = workbook.DataSorter;
sorter.AddKey(0, SortOrder.Ascending);
sorter.Sort(worksheet.Cells, 0, 0, 3, 0);
workbook.Save("StringComparisonDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error during string comparison: {ex.Message}");
}
}
private class CustomGlobalizationSettings : GlobalizationSettings
{
public override int Compare(string v1, string v2, bool ignoreCase)
{
return String.Compare(v1, v2, ignoreCase);
}
}
}
}
```
### See Also
* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
