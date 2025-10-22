##GlobalizationSettings.GetStandardHeaderFooterFontStyleName
GlobalizationSettings method. Gets standard English font style nameRegular Bold Italic for Header/Footer according to given locale font style name
## GlobalizationSettings.GetStandardHeaderFooterFontStyleName method
Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name.
```csharp
public virtual string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | String | Locale font style name for Header/Footer. |
### Return Value
Standard English font style name(Regular, Bold, Italic)
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class GlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings instance
var globalizationSettings = new CustomGlobalizationSettings();
try
{
// Demonstrate method call with parameter type (String)
string localStyle = "CustomBold";
string standardStyle = globalizationSettings.GetStandardHeaderFooterFontStyleName(localStyle);
Console.WriteLine($"Converted font style: {localStyle} -> {standardStyle}");
// Apply globalization settings to the workbook
workbook.Settings.GlobalizationSettings = globalizationSettings;
// Set header with custom font style that will be converted
// Use SetHeader method with section parameter (0 = left, 1 = center, 2 = right)
worksheet.PageSetup.SetHeader(1, "&\"Arial\"&\"CustomBold\"&12Header Text");
// Save the workbook to show effect
workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
}
}
}
// Custom globalization settings implementation
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
{
// Convert custom font style names to standard names
return localfontStyleName switch
{
"CustomBold" => "Bold",
"CustomItalic" => "Italic",
_ => base.GetStandardHeaderFooterFontStyleName(localfontStyleName)
};
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
