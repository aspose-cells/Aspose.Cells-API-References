##Font.ScriptOffset
Font property. Gets and sets the script offsetin unit of percentage
## Font.ScriptOffset property
Gets and sets the script offset,in unit of percentage
```csharp
public double ScriptOffset { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyScriptOffsetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set its value
Cell cell = worksheet.Cells["A1"];
cell.PutValue("ScriptOffset Demo");
// Get the style and font of the cell
Style style = cell.GetStyle();
Font font = style.Font;
// Set ScriptOffset to demonstrate subscript/superscript effect
font.ScriptOffset = 10; // Positive for superscript, negative for subscript
font.IsSuperscript = true; // Enable superscript
// Apply the modified style back to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("FontScriptOffsetDemo.xlsx");
// Verify the ScriptOffset value
Console.WriteLine("ScriptOffset value: " + font.ScriptOffset);
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
