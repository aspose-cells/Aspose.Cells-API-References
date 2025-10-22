##Font.Charset
Font property. Represent the character set
## Font.Charset property
Represent the character set.
```csharp
public int Charset { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyCharsetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with specific font properties including charset
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 12;
style.Font.Charset = 1; // ANSI_CHARSET
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.SetStyle(style);
cell.PutValue("Text with ANSI charset");
// Create another style with different charset
Style style2 = workbook.CreateStyle();
style2.Font.Name = "Times New Roman";
style2.Font.Size = 12;
style2.Font.Charset = 2; // DEFAULT_CHARSET
// Apply the second style to another cell
Cell cell2 = worksheet.Cells["A2"];
cell2.SetStyle(style2);
cell2.PutValue("Text with DEFAULT charset");
// Save the workbook
workbook.Save("FontCharsetDemo.xlsx");
// Verify the charset properties
Console.WriteLine("Cell A1 Font Charset: " + cell.GetStyle().Font.Charset);
Console.WriteLine("Cell A2 Font Charset: " + cell2.GetStyle().Font.Charset);
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
