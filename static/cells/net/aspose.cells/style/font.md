##Style.Font
Style property. Gets a Font object
## Style.Font property
Gets a `Font` object.
```csharp
public Font Font { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StylePropertyFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Access cell B4 and set its font to bold
Cell b4 = cells["B4"];
Style b4Style = b4.GetStyle();
b4Style.Font.IsBold = true;
b4.SetStyle(b4Style);
// Access cell C4 and ensure its font is not bold
Cell c4 = cells["C4"];
Style c4Style = c4.GetStyle();
c4Style.Font.IsBold = false;
c4.SetStyle(c4Style);
// Access cell D4 and set its font to bold with a different color
Cell d4 = cells["D4"];
Style d4Style = d4.GetStyle();
d4Style.Font.IsBold = true;
d4Style.Font.Color = Color.Red;
d4.SetStyle(d4Style);
// Verify the font properties
Console.WriteLine("B4 Font Bold: " + b4.GetStyle().Font.IsBold);
Console.WriteLine("C4 Font Bold: " + c4.GetStyle().Font.IsBold);
Console.WriteLine("D4 Font Bold: " + d4.GetStyle().Font.IsBold);
Console.WriteLine("D4 Font Color: " + d4.GetStyle().Font.Color);
// Save the workbook
workbook.Save("FontPropertyDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
