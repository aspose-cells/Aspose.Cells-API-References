##Style.IndentLevel
Style property. Represents the indent level for the cell or range. Can only be an integer from 0 to 250
## Style.IndentLevel property
Represents the indent level for the cell or range. Can only be an integer from 0 to 250.
```csharp
public int IndentLevel { get; set; }
```
### Remarks
If text horizontal alignment type is set to value other than left or right, indent level will be reset to zero.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyIndentLevelDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set different indent levels for cells
for (int i = 0; i < 16; i++)
{
Cell cell = cells[i, 0];
Style style = cell.GetStyle();
style.IndentLevel = i;
style.HorizontalAlignment = TextAlignmentType.Left;
cell.SetStyle(style);
cell.PutValue($"Indent Level {i}");
}
// Save the workbook
workbook.Save("IndentLevelDemo.xlsx");
Console.WriteLine("Workbook saved with different indent levels.");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
