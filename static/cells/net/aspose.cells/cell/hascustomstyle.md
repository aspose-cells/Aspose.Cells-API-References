##Cell.HasCustomStyle
Cell property. Indicates whether this cell has custom style settingsdifferent from the default one inherited from corresponding row column or workbook
## Cell.HasCustomStyle property
Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook).
```csharp
public bool HasCustomStyle { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellPropertyHasCustomStyleDemo
{
public static void Run()
{
// Create a new workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Check HasCustomStyle");
// Display initial HasCustomState value (inherits default style)
Console.WriteLine("Initial HasCustomStyle: " + cell.HasCustomStyle);
// Create a custom style and apply it to the cell
Style customStyle = workbook.CreateStyle();
customStyle.Font.IsBold = true;
cell.SetStyle(customStyle);
// Verify HasCustomStyle is true after style modification
Console.WriteLine("After applying custom style - HasCustomStyle: " + cell.HasCustomStyle);
// Save the workbook with the custom style applied
workbook.Save("CellCustomStyleDemo.xlsx");
// Reset the cell's style to the workbook's default style
Style defaultStyle = workbook.DefaultStyle;
cell.SetStyle(defaultStyle);
// Verify HasCustomStyle is false after reverting to default
Console.WriteLine("After resetting to default style - HasCustomStyle: " + cell.HasCustomStyle);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
