##StyleFlag.NumberFormat
StyleFlag property. Number format setting will be applied
## StyleFlag.NumberFormat property
Number format setting will be applied.
```csharp
public bool NumberFormat { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyNumberFormatDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set cell value
sheet.Cells[0, 0].Value = 1234.56;
// Create custom number format style
Style style = workbook.CreateStyle();
style.Custom = "_-€ #,##0.00;[Red]_-€ -#,##0.00";
// Apply only number format using StyleFlag
StyleFlag styleFlag = new StyleFlag();
styleFlag.NumberFormat = true;
// Apply the style to cell range (fully qualify Range type)
Aspose.Cells.Range range = sheet.Cells.CreateRange(0, 0, 1, 1);
range.ApplyStyle(style, styleFlag);
// Save and verify
workbook.Save("output_number_format.ods");
// Reload to verify
Workbook verifyWorkbook = new Workbook("output_number_format.ods");
Worksheet verifySheet = verifyWorkbook.Worksheets[0];
Console.WriteLine("Applied Number Format: " + verifySheet.Cells["A1"].GetStyle().Custom);
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
