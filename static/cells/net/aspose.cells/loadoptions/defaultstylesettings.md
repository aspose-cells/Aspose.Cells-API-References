##LoadOptions.DefaultStyleSettings
LoadOptions property. Gets the default style settings for initializing styles of the workbook
## LoadOptions.DefaultStyleSettings property
Gets the default style settings for initializing styles of the workbook
```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyDefaultStyleSettingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set load options with default style settings
LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
// Create a worksheet and get cells
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set values to demonstrate default style
cells["A1"].PutValue("Default Style Applied");
cells["A2"].PutValue("Should have bottom alignment");
// Create a cell with custom style (to contrast with default)
Cell customCell = cells["B1"];
customCell.PutValue("Custom Style");
Style customStyle = customCell.GetStyle();
customStyle.VerticalAlignment = TextAlignmentType.Center;
customCell.SetStyle(customStyle);
// Save the workbook
workbook.Save("DefaultStyleSettingsDemo.xlsx");
// Verify the styles
Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
Console.WriteLine("B1 Vertical Alignment: " + cells["B1"].GetStyle().VerticalAlignment);
}
}
}
```
### See Also
* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
