##SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName
SettableGlobalizationSettings method. Gets standard English font style nameRegular Bold Italic for Header/Footer according to given locale font style name
## SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName method
Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name.
```csharp
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
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
public class SettableGlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Set a standard header/footer font style name mapping
settings.SetStandardHeaderFooterFontStyleName("MyLocalFontStyle", "Arial");
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
try
{
// Call the GetStandardHeaderFooterFontStyleName method with a local font style name
string standardFontStyle = settings.GetStandardHeaderFooterFontStyleName("MyLocalFontStyle");
// Display the result
Console.WriteLine($"Standard font style name for 'MyLocalFontStyle': {standardFontStyle}");
// Create a header with the local font style name
worksheet.PageSetup.SetHeader(1, "&\"MyLocalFontStyle\"&12Test Header");
// Show the effect in the spreadsheet
Console.WriteLine("Header set with local font style name 'MyLocalFontStyle'");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
