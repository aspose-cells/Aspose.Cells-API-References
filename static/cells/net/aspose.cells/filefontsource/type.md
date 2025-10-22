##FileFontSource.Type
FileFontSource property. Returns the type of the font source
## FileFontSource.Type property
Returns the type of the font source.
```csharp
public override FontSourceType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFontSourcePropertyTypeDemo
{
public static void Run()
{
string fontFilePath = "CustomFont.ttf";
// Create a FileFontSource instance
FileFontSource fontSource = new FileFontSource(fontFilePath);
// Demonstrate Type property usage
Console.WriteLine("Font Source Type: " + fontSource.Type);
// Create workbook and apply font
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cell cell = sheet.Cells["A1"];
cell.PutValue("Text with custom font");
Style style = cell.GetStyle();
style.Font.Name = "CustomFont";
cell.SetStyle(style);
workbook.Save("FontSourceDemo.xlsx");
}
}
}
```
### See Also
* enum [FontSourceType](../../fontsourcetype/)
* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
