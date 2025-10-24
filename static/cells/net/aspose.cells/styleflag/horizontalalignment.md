##StyleFlag.HorizontalAlignment
StyleFlag property. Horizontal alignment setting will be applied
## StyleFlag.HorizontalAlignment property
Horizontal alignment setting will be applied.
```csharp
public bool HorizontalAlignment { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyHorizontalAlignmentDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data in cells
worksheet.Cells["A1"].PutValue("Left Aligned");
worksheet.Cells["B1"].PutValue("Center Aligned");
worksheet.Cells["C1"].PutValue("Right Aligned");
// Create styles with different horizontal alignments
Style styleLeft = workbook.CreateStyle();
styleLeft.HorizontalAlignment = TextAlignmentType.Left;
Style styleCenter = workbook.CreateStyle();
styleCenter.HorizontalAlignment = TextAlignmentType.Center;
Style styleRight = workbook.CreateStyle();
styleRight.HorizontalAlignment = TextAlignmentType.Right;
// Create style flags to only apply horizontal alignment
StyleFlag flag = new StyleFlag();
flag.HorizontalAlignment = true;
// Apply styles to ranges
Aspose.Cells.Range rangeLeft = worksheet.Cells.CreateRange("A1:A1");
rangeLeft.ApplyStyle(styleLeft, flag);
Aspose.Cells.Range rangeCenter = worksheet.Cells.CreateRange("B1:B1");
rangeCenter.ApplyStyle(styleCenter, flag);
Aspose.Cells.Range rangeRight = worksheet.Cells.CreateRange("C1:C1");
rangeRight.ApplyStyle(styleRight, flag);
// Save the workbook
workbook.Save("HorizontalAlignmentDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
