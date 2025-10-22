##DefaultStyleSettings.HorizontalAlignment
DefaultStyleSettings property. Gets/Sets the default value for horizontal alignment
## DefaultStyleSettings.HorizontalAlignment property
Gets/Sets the default value for horizontal alignment
```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DefaultStyleSettingsPropertyHorizontalAlignmentDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;
// Set horizontal alignment to demonstrate the property
defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Centered Text";
worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });
workbook.Save("HorizontalAlignmentDemo.xlsx");
}
}
}
```
### See Also
* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
