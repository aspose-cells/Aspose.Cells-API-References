##GlobalizationSettings.GetCollationKey
GlobalizationSettings method. Transforms the string into a comparable object according to certain collation rules
## GlobalizationSettings.GetCollationKey method
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
public class GlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
CustomGlobalizationSettings settings = new CustomGlobalizationSettings();
workbook.Settings.GlobalizationSettings = settings;
string inputString = "SampleText";
bool ignoreCase = true;
try
{
IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
Console.WriteLine($"Collation key for '{inputString}' (ignore case {ignoreCase}): {collationKey}");
worksheet.Cells["A1"].Value = "Cherry";
worksheet.Cells["A2"].Value = "apple";
worksheet.Cells["A3"].Value = "Banana";
DataSorter sorter = workbook.DataSorter;
sorter.CaseSensitive = !ignoreCase;
sorter.Sort(worksheet.Cells, 0, 0, 2, 0);
Console.WriteLine("\nSorted data:");
int minDataRow = worksheet.Cells.MinDataRow;
int maxDataRow = worksheet.Cells.MaxDataRow;
for (int row = minDataRow; row <= maxDataRow; row++)
{
Cell cell = worksheet.Cells[row, 0];
Console.WriteLine(cell.StringValue);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCollationKey: {ex.Message}");
}
workbook.Save("GlobalizationSettingsMethodGetCollationKeyDemo.xlsx");
}
}
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override IComparable GetCollationKey(string v, bool ignoreCase)
{
return ignoreCase ? v.ToLowerInvariant() : v;
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
