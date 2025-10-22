##Font.IsSuperscript
Font property. Gets or sets a value indicating whether the font is super script
## Font.IsSuperscript property
Gets or sets a value indicating whether the font is super script.
```csharp
public bool IsSuperscript { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyIsSuperscriptDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add text to cell A1
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Normal Text Superscript Text");
// Format part of the text as superscript
FontSetting setting = cell.Characters(12, 11);
setting.Font.IsSuperscript = true;
// Save the workbook
workbook.Save("FontIsSuperscriptDemo.xlsx");
// Verify the superscript setting
Console.WriteLine("IsSuperscript property: " + setting.Font.IsSuperscript);
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
