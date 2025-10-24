##StyleFlag.FontSize
StyleFlag property. Font size setting will be applied
## StyleFlag.FontSize property
Font size setting will be applied.
```csharp
public bool FontSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyFontSizeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Text");
Style style = workbook.CreateStyle();
style.Font.Size = 18;
style.Font.IsBold = true;
StyleFlag styleFlag = new StyleFlag
{
FontSize = true,
FontBold = true
};
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A1");
range.ApplyStyle(style, styleFlag);
workbook.Save("FontSizeDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
