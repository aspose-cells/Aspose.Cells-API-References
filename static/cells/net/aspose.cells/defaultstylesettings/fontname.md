##DefaultStyleSettings.FontName
DefaultStyleSettings property. Gets/Sets the default font name for the workbook
## DefaultStyleSettings.FontName property
Gets/Sets the default font name for the workbook
```csharp
public string FontName { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DefaultStyleSettingsPropertyFontNameDemo
{
public static void Run()
{
// Create load options and set font name
LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
loadOptions.DefaultStyleSettings.FontName = "SimSun";
// Create a new workbook with the load options
Workbook workbook = new Workbook();
workbook.DefaultStyle.Font.Name = loadOptions.DefaultStyleSettings.FontName;
// Access the default style and verify font name
Style defaultStyle = workbook.DefaultStyle;
Console.WriteLine("Default Font Name: " + defaultStyle.Font.Name);
// Create a worksheet and set cell value
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Font Name Test");
// Save the workbook
using (MemoryStream stream = new MemoryStream())
{
workbook.Save(stream, SaveFormat.Xlsx);
Console.WriteLine("Workbook saved with default font: SimSun");
}
}
}
}
```
### See Also
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
