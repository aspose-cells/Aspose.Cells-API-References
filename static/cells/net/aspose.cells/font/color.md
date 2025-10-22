##Font.Color
Font property. Gets or sets the Color of the font
## Font.Color property
Gets or sets the Color of the font.
```csharp
public Color Color { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FontPropertyColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set HTML with different font colors and styles
Cell cell = worksheet.Cells["A1"];
cell.HtmlString = "<font color='Red'>Red Text</font> <font color='#0000FF'>Blue Text</font> <font style='color:#00FF00;text-decoration: underline;'>Green Underlined</font>";
// Get rich text formatting
FontSetting[] richText = cell.GetCharacters();
// Verify and demonstrate color properties
Console.WriteLine("First segment color: " + richText[0].Font.Color);
Console.WriteLine("Second segment color: " + richText[1].Font.Color);
Console.WriteLine("Third segment underline: " + richText[2].Font.Underline);
// Save the workbook
workbook.Save("FontColorDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
