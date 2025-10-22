##Row.HasCustomStyle
Row property. Indicates whether this row has custom style settingsdifferent from the default one inherited from workbook
## Row.HasCustomStyle property
Indicates whether this row has custom style settings(different from the default one inherited from workbook).
```csharp
public bool HasCustomStyle { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RowPropertyHasCustomStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create and customize a style
Style customStyle = workbook.CreateStyle();
customStyle.BackgroundColor = Color.LightBlue;
customStyle.Pattern = BackgroundType.Solid;
// Access first row
Row row = worksheet.Cells.Rows[0];
// Apply custom style to the row
row.ApplyStyle(customStyle, new StyleFlag { All = true });
// Check if row has custom style (should be true)
bool hasCustomStyle = row.HasCustomStyle;
Console.WriteLine("Row has custom style: " + hasCustomStyle);
// Save the workbook
workbook.Save("RowHasCustomStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
