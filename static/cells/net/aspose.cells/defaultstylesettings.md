##Class DefaultStyleSettings
Aspose.Cells.DefaultStyleSettings class. Settings for the default values of workbooks style properties
## DefaultStyleSettings class
Settings for the default values of workbook's style properties.
```csharp
public class DefaultStyleSettings
```
## Properties
| Name | Description |
| --- | --- |
| [BuiltInPreference](../../aspose.cells/defaultstylesettings/builtinpreference/) { get; set; } | Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style. |
| [FontName](../../aspose.cells/defaultstylesettings/fontname/) { get; set; } | Gets/Sets the default font name for the workbook |
| [FontSize](../../aspose.cells/defaultstylesettings/fontsize/) { get; set; } | Gets/Sets the default standard font size for the workbook. |
| [HorizontalAlignment](../../aspose.cells/defaultstylesettings/horizontalalignment/) { get; set; } | Gets/Sets the default value for horizontal alignment |
| [VerticalAlignment](../../aspose.cells/defaultstylesettings/verticalalignment/) { get; set; } | Gets/Sets the default value for vertical alignment |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DefaultStyleSettingsDemo
{
public static void DefaultStyleSettingsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the default style settings of the workbook
DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;
// Setting properties
defaultStyleSettings.BuiltInPreference = false;
defaultStyleSettings.FontName = "Arial";
defaultStyleSettings.FontSize = 12.0;
defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
defaultStyleSettings.VerticalAlignment = TextAlignmentType.Center;
// Apply the default style settings to the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });
// Save the workbook
workbook.Save("DefaultStyleSettingsExample.xlsx");
workbook.Save("DefaultStyleSettingsExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
