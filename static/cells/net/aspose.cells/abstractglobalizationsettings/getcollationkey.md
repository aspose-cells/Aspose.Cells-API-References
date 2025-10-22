##AbstractGlobalizationSettings.GetCollationKey
AbstractGlobalizationSettings method. Transforms the string into a comparable object according to certain collation rules
## AbstractGlobalizationSettings.GetCollationKey method
Transforms the string into a comparable object according to certain collation rules.
```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```
| Parameter | Type | Description |
| --- | --- | --- |
| v | String | String value needs to be compared with others. |
| ignoreCase | Boolean | whether ignore case when comparing values |
### Return Value
Object can be used to compare or sort string values
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AbstractGlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
{
public static void Run()
{
// Create custom globalization settings that override the GetCollationKey method
var settings = new CustomGlobalizationSettings();
// Create a workbook with custom globalization settings
Workbook workbook = new Workbook();
workbook.Settings.GlobalizationSettings = settings;
// Prepare string for collation key
string inputString = "Sample Text";
bool ignoreCase = true;
try
{
// Call GetCollationKey directly
IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
Console.WriteLine($"Original string: {inputString}");
Console.WriteLine($"Collation key: {collationKey}");
Console.WriteLine($"Ignore case: {ignoreCase}");
// Demonstrate effect by using in worksheet operations
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("banana");
worksheet.Cells["A3"].PutValue("Cherry");
// Sorting will use the GetCollationKey internally
DataSorter sorter = workbook.DataSorter;
sorter.AddKey(0, SortOrder.Descending);
sorter.Sort(worksheet.Cells, 0, 0, 2, 0);
workbook.Save("GetCollationKeyDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error during GetCollationKey operation: {ex.Message}");
}
}
private class CustomGlobalizationSettings : GlobalizationSettings
{
public override IComparable GetCollationKey(string v, bool ignoreCase)
{
return ignoreCase ? v.ToLowerInvariant() : v;
}
}
}
}
```
### See Also
* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
