##FontConfigs.SetFontFolder
FontConfigs method. Sets the fonts folder
## FontConfigs.SetFontFolder method
Sets the fonts folder
```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolder | String | The folder that contains TrueType fonts. |
| recursive | Boolean | Determines whether or not to scan subfolders. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontConfigsMethodSetFontFolderWithStringBooleanDemo
{
public static void Run()
{
// Initialize a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some text to cell A1
worksheet.Cells["A1"].PutValue("Sample Text with Custom Font");
// Set custom font folder and specify whether to include subfolders
FontConfigs.SetFontFolder("Fonts", true);
// Apply a font style that might use fonts from the custom folder
Style style = worksheet.Cells["A1"].GetStyle();
style.Font.Name = "CustomFont"; // Assuming "CustomFont" exists in the Fonts folder
style.Font.Size = 14;
worksheet.Cells["A1"].SetStyle(style);
// Save the workbook to PDF
workbook.Save("output.pdf", SaveFormat.Pdf);
}
}
}
```
### See Also
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
