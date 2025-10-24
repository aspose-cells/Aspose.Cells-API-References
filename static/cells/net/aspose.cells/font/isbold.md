##Font.IsBold
Font property. Gets or sets a value indicating whether the font is bold
## Font.IsBold property
Gets or sets a value indicating whether the font is bold.
```csharp
public bool IsBold { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyIsBoldDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set its value
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Bold Text Demo");
// Get cell's style and set font to bold
Style style = cell.GetStyle();
style.Font.IsBold = true;
cell.SetStyle(style);
// Save the workbook
workbook.Save("FontIsBoldDemo.xlsx");
// Verify the bold property
Workbook loadedWorkbook = new Workbook("FontIsBoldDemo.xlsx");
Style loadedStyle = loadedWorkbook.Worksheets[0].Cells["A1"].GetStyle();
Console.WriteLine("IsBold property: " + loadedStyle.Font.IsBold);
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
