##Font.DoubleSize
Font property. Gets and sets the double size of the font
## Font.DoubleSize property
Gets and sets the double size of the font.
```csharp
public double DoubleSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyDoubleSizeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
Style style = cell.GetStyle();
style.Font.DoubleSize = 10.5;
cell.SetStyle(style);
Console.WriteLine("Font DoubleSize set to: " + cell.GetStyle().Font.DoubleSize);
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
