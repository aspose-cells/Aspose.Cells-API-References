##Font.IsItalic
Font property. Gets or sets a value indicating whether the font is italic
## Font.IsItalic property
Gets or sets a value indicating whether the font is italic.
```csharp
public bool IsItalic { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyIsItalicDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the default style
Style style = workbook.DefaultStyle;
// Set font properties including IsItalic
style.Font.Name = "Arial";
style.Font.Size = 12;
style.Font.IsBold = true;
style.Font.IsItalic = true;
// Apply the style to cell A1
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
cell.SetStyle(style);
cell.PutValue("Italic Text Example");
// Save the workbook
workbook.Save("FontPropertyIsItalicDemo.xlsx");
// Verify the italic property
Console.WriteLine("Font is italic: " + cell.GetStyle().Font.IsItalic);
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
