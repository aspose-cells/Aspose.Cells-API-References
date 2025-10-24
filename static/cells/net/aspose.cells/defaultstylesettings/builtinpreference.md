##DefaultStyleSettings.BuiltInPreference
DefaultStyleSettings property. Indicates whether property for number format is preferable when the style defines both builtin number and custom pattern. Default value is false that means by default custom pattern will be used to format values as long as it is not empty for one style
## DefaultStyleSettings.BuiltInPreference property
Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style.
```csharp
public bool BuiltInPreference { get; set; }
```
### Remarks
When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DefaultStyleSettingsPropertyBuiltInPreferenceDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access default style settings
DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;
// Demonstrate BuiltInPreference property
defaultStyleSettings.BuiltInPreference = false;
defaultStyleSettings.FontName = "Arial";
defaultStyleSettings.FontSize = 12;
// Apply to worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Text");
// Save the workbook
workbook.Save("BuiltInPreferenceDemo.xlsx");
}
}
}
```
### See Also
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
