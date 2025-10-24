##Font.SchemeType
Font property. Gets and sets the scheme type of the font
## Font.SchemeType property
Gets and sets the scheme type of the font.
```csharp
public FontSchemeType SchemeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertySchemeTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample Text");
Font font = cell.GetStyle().Font;
font.SchemeType = FontSchemeType.Minor;
font.Name = "Calibri";
font.Size = 12;
workbook.Save("FontSchemeTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
