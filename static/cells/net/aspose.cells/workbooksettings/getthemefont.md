##WorkbookSettings.GetThemeFont
WorkbookSettings method. Gets the default theme font name
## WorkbookSettings.GetThemeFont method
Gets the default theme font name.
```csharp
public string GetThemeFont(FontSchemeType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | FontSchemeType | The scheme type of the font. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsMethodGetThemeFontWithFontSchemeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the default theme font for minor scheme type
string minorFont = workbook.Settings.GetThemeFont(FontSchemeType.Minor);
Console.WriteLine("Minor theme font: " + minorFont);
// Get the default theme font for major scheme type
string majorFont = workbook.Settings.GetThemeFont(FontSchemeType.Major);
Console.WriteLine("Major theme font: " + majorFont);
// Save the workbook
workbook.Save("ThemeFontExample.xlsx");
}
}
}
```
### See Also
* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
