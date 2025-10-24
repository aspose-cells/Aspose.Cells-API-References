##GlobalizationSettings.GetLocalBuiltInName
GlobalizationSettings method. Gets the locale dependent text for builtin Name according to given standard text
## GlobalizationSettings.GetLocalBuiltInName method
Gets the locale dependent text for built-in Name according to given standard text.
```csharp
public virtual string GetLocalBuiltInName(string standardName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) text of built-in Name. |
### Return Value
Locale dependent text. The locale was specified by the Workbook for which this settings is used.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class GlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
try
{
string standardName = "Total";
string localizedName = ((CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings).GetLocalBuiltInName(standardName);
Console.WriteLine($"Standard Name: {standardName}");
Console.WriteLine($"Localized Name: {localizedName}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
}
workbook.Save("LocalizedBuiltInNameDemo.xlsx");
}
}
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetLocalBuiltInName(string standardName)
{
switch (standardName)
{
case "Total":
return "LocalizedTotal";
case "Average":
return "LocalizedAverage";
default:
return base.GetLocalBuiltInName(standardName);
}
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
