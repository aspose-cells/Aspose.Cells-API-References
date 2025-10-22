##ReplaceOptions.FontSettings
ReplaceOptions property. The rich formatted settings for the replaced text
## ReplaceOptions.FontSettings property
The rich formatted settings for the replaced text.
```csharp
public FontSetting[] FontSettings { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReplaceOptionsPropertyFontSettingsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample text in cell A1
worksheet.Cells["A1"].Value = "Sample text for replacement";
// Create replace options with font settings
ReplaceOptions options = new ReplaceOptions();
options.MatchEntireCellContents = false;
// Create font setting for the replacement text
FontSetting fontSetting = new FontSetting(0, 8, workbook.Worksheets);
fontSetting.Font.IsBold = true;
fontSetting.Font.Color = Color.Blue;
// Apply font settings to replace options
options.FontSettings = new FontSetting[] { fontSetting };
// Perform the replacement
workbook.Replace("text", "REPLACED", options);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
