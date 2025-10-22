##LoadOptions.StandardFontSize
LoadOptions property. Sets the default standard font size
## LoadOptions.StandardFontSize property
Sets the default standard font size.
```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyStandardFontSizeDemo
{
public static void Run()
{
// Create HTML load options and set StandardFontSize
HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
loadOptions.StandardFont = "Calibri";
loadOptions.StandardFontSize = 11;
// Load workbook with the options
Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
// Access first worksheet and cells
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set some sample text and verify font properties
cells["A1"].PutValue("Sample Text");
Style style = cells["A1"].GetStyle();
Console.WriteLine("Font Name: " + style.Font.Name);
Console.WriteLine("Font Size: " + style.Font.Size);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
