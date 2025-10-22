##StyleFlag.TextDirection
StyleFlag property. Text direction setting will be applied
## StyleFlag.TextDirection property
Text direction setting will be applied.
```csharp
public bool TextDirection { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class StyleFlagPropertyTextDirectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set some text
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample Text with TextDirection");
// Create a style and set text direction
Style style = workbook.CreateStyle();
style.TextDirection = TextDirectionType.Context;
// Create a style flag and enable TextDirection flag
StyleFlag styleFlag = new StyleFlag();
styleFlag.TextDirection = true;
// Apply the style to the cell with the style flag
cell.SetStyle(style, styleFlag);
// Display current text direction
Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);
// Change text direction and apply again
style.TextDirection = TextDirectionType.LeftToRight;
cell.SetStyle(style, styleFlag);
Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);
// Save the workbook
workbook.Save("TextDirectionDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
