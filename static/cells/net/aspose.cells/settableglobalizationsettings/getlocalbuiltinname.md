##SettableGlobalizationSettings.GetLocalBuiltInName
SettableGlobalizationSettings method. Gets the locale dependent text for builtin Name according to given standard text
## SettableGlobalizationSettings.GetLocalBuiltInName method
Gets the locale dependent text for built-in Name according to given standard text.
```csharp
public override string GetLocalBuiltInName(string standardName)
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
public class SettableGlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SettableGlobalizationSettings
SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
try
{
// Call the GetLocalBuiltInName method with a standard built-in name
string standardName = "SUM";
string localName = globalizationSettings.GetLocalBuiltInName(standardName);
// Display the result
Console.WriteLine($"Standard name: {standardName}, Local name: {localName}");
// Set a custom local name for the standard built-in name
globalizationSettings.SetLocalBuiltInName(standardName, "CustomSum", true);
// Get the local name again after setting it
localName = globalizationSettings.GetLocalBuiltInName(standardName);
Console.WriteLine($"After setting - Standard name: {standardName}, Local name: {localName}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodGetLocalBuiltInNameDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
