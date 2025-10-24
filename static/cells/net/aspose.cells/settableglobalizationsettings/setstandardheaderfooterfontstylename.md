##SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName
SettableGlobalizationSettings method. Sets the locale dependent function name according to given standard function name
## SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName method
Sets the locale dependent function name according to given standard function name.
```csharp
public void SetStandardHeaderFooterFontStyleName(string localfontStyleName, string standardName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | String | Locale font style name for Header/Footer. |
| standardName | String | Standard(en-US locale) function name. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodSetStandardHeaderFooterFontStyleNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create page setup options for the worksheet
PageSetup pageSetup = worksheet.PageSetup;
// Set a header with some text
pageSetup.SetHeader(0, "&\"Arial\"&12This is a header");
// Create globalization settings instance
SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
try
{
// Call the SetStandardHeaderFooterFontStyleName method
globalizationSettings.SetStandardHeaderFooterFontStyleName("Arial", "Times New Roman");
// Apply the globalization settings to the workbook
workbook.Settings.GlobalizationSettings = globalizationSettings;
Console.WriteLine("SetStandardHeaderFooterFontStyleName method executed successfully with parameters (\"Arial\", \"Times New Roman\")");
// The effect will be visible when the document is rendered or printed
// The font style "Arial" in headers/footers will be treated as "Times New Roman"
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetStandardHeaderFooterFontStyleName method: {ex.Message}");
}
// Save the result
workbook.Save("MethodSetStandardHeaderFooterFontStyleNameDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
