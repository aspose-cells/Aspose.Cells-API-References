##Font.ArgbColor
Font property. Gets and sets the color with a 32bit ARGB value
## Font.ArgbColor property
Gets and sets the color with a 32-bit ARGB value.
```csharp
public int ArgbColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyArgbColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cells and set values with different font colors
Cell cell1 = worksheet.Cells["A1"];
cell1.PutValue("Red Text");
Style style1 = cell1.GetStyle();
style1.Font.ArgbColor = unchecked((int)0xFFFF0000); // Red
cell1.SetStyle(style1);
Cell cell2 = worksheet.Cells["A2"];
cell2.PutValue("Blue Text");
Style style2 = cell2.GetStyle();
style2.Font.ArgbColor = unchecked((int)0xFF0000FF); // Blue
cell2.SetStyle(style2);
Cell cell3 = worksheet.Cells["A3"];
cell3.PutValue("Green Text");
Style style3 = cell3.GetStyle();
style3.Font.ArgbColor = unchecked((int)0xFF00FF00); // Green
cell3.SetStyle(style3);
// Verify and output the colors
Console.WriteLine("Cell A1 Font Color: 0x{0:X8}", worksheet.Cells["A1"].GetStyle().Font.ArgbColor);
Console.WriteLine("Cell A2 Font Color: 0x{0:X8}", worksheet.Cells["A2"].GetStyle().Font.ArgbColor);
Console.WriteLine("Cell A3 Font Color: 0x{0:X8}", worksheet.Cells["A3"].GetStyle().Font.ArgbColor);
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
