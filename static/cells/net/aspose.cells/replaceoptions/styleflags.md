##ReplaceOptions.StyleFlags
ReplaceOptions property. Gets and sets flags of applying font settings
## ReplaceOptions.StyleFlags property
Gets and sets flags of applying font settings.
```csharp
public StyleFlag[] StyleFlags { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ReplaceOptionsPropertyStyleFlagsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample text to cell
Cell cell = worksheet.Cells["A1"];
cell.PutValue("test text");
// Create replacement options
ReplaceOptions options = new ReplaceOptions();
options.MatchEntireCellContents = false;
options.CaseSensitive = false;
// Create font setting and style flag
string replacementText = "new text";
FontSetting setting = new FontSetting(0, replacementText.Length, workbook.Worksheets);
StyleFlag styleFlag = new StyleFlag();
// Configure font and style
setting.Font.Color = Color.Red;
setting.Font.Underline = FontUnderlineType.Single;
styleFlag.FontColor = true;
styleFlag.FontUnderline = true;
// Apply settings to options
options.FontSettings = new FontSetting[] { setting };
options.StyleFlags = new StyleFlag[] { styleFlag };
// Perform replacement
workbook.Replace("test", replacementText, options);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
