##StyleFlag.StyleFlag
StyleFlag constructor. Constructs an object with all flags as false
## StyleFlag constructor
Constructs an object with all flags as false.
```csharp
public StyleFlag()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a bold style
Style boldStyle = workbook.CreateStyle();
boldStyle.Font.IsBold = true;
// Apply style to row 9 with StyleFlag constructor
worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });
// Put value in cell and verify style
worksheet.Cells[9, 0].PutValue("Bold Text");
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("Style applied successfully using StyleFlag constructor.");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
