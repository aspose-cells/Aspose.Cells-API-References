##Class FileFontSource
Aspose.Cells.FileFontSource class. Represents the single TrueType font file stored in the file system
## FileFontSource class
Represents the single TrueType font file stored in the file system.
```csharp
public class FileFontSource : FontSourceBase
```
## Constructors
| Name | Description |
| --- | --- |
| [FileFontSource](filefontsource/)(string) | Ctor. |
## Properties
| Name | Description |
| --- | --- |
| [FilePath](../../aspose.cells/filefontsource/filepath/) { get; } | Path to font file. |
| override [Type](../../aspose.cells/filefontsource/type/) { get; } | Returns the type of the font source. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FileFontSourceDemo
{
public static void FileFontSourceExample()
{
// Specify the path to the TrueType font file
string fontFilePath = "C:\\Fonts\\CustomFont.ttf";
// Create a FileFontSource instance
FileFontSource fontSource = new FileFontSource(fontFilePath);
// Display the font source type and file path
Console.WriteLine("Font Source Type: " + fontSource.Type);
Console.WriteLine("Font File Path: " + fontSource.FilePath);
// Create a Workbook object
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set a cell value
Cell cell = sheet.Cells["A1"];
cell.PutValue("Hello, Aspose!");
// Apply the custom font to the cell
Style style = cell.GetStyle();
style.Font.Name = "CustomFont"; // Use the name of the font
cell.SetStyle(style);
// Save the workbook
workbook.Save("FileFontSourceExample.xlsx");
workbook.Save("FileFontSourceExample.pdf");
}
}
}
```
### See Also
* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
