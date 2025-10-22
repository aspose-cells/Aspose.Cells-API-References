##Font.CapsType
Font property. Gets and sets the text caps type
## Font.CapsType property
Gets and sets the text caps type.
```csharp
public TextCapsType CapsType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyCapsTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
cell.PutValue("sample text");
Style style = cell.GetStyle();
style.Font.CapsType = TextCapsType.All;
cell.SetStyle(style);
workbook.Save("FontCapsTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TextCapsType](../../textcapstype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
