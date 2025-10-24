##Font.Size
Font property. Gets or sets the size of the font
## Font.Size property
Gets or sets the size of the font.
```csharp
public int Size { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertySizeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set text with different font sizes
Cell cell1 = worksheet.Cells["A1"];
cell1.Value = "Text with size 12";
Style style1 = workbook.CreateStyle();
style1.Font.Size = 12;
cell1.SetStyle(style1);
Cell cell2 = worksheet.Cells["A3"];
cell2.Value = "Text with size 16";
Style style2 = workbook.CreateStyle();
style2.Font.Size = 16;
cell2.SetStyle(style2);
// Save the workbook
workbook.Save("FontSizeDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
