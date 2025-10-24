##StyleFlag.Alignments
StyleFlag property. Alignment setting will be applied
## StyleFlag.Alignments property
Alignment setting will be applied.
```csharp
public bool Alignments { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class StyleFlagPropertyAlignmentsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set some text
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample Text");
// Create a style object and set alignment properties
Style style = workbook.CreateStyle();
style.HorizontalAlignment = TextAlignmentType.Center;
style.VerticalAlignment = TextAlignmentType.Center;
style.RotationAngle = 45;
// Create a style flag and enable alignment properties
StyleFlag styleFlag = new StyleFlag();
styleFlag.Alignments = true;
// Apply the style to the cell with the style flag
cell.SetStyle(style, styleFlag);
// Display the current alignment settings
Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);
// Modify the style flag to disable alignment properties
styleFlag.Alignments = false;
// Create a new style with different alignment
Style newStyle = workbook.CreateStyle();
newStyle.HorizontalAlignment = TextAlignmentType.Right;
newStyle.VerticalAlignment = TextAlignmentType.Top;
newStyle.RotationAngle = 0;
// Apply the new style - alignments won't change because flag is false
cell.SetStyle(newStyle, styleFlag);
// Display the unchanged alignment settings
Console.WriteLine("After applying new style with Alignments=false:");
Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);
// Save the workbook
workbook.Save("StyleFlagAlignmentsDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
