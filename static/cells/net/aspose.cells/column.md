##Class Column
Aspose.Cells.Column class. Represents a single column in a worksheet
## Column class
Represents a single column in a worksheet.
```csharp
public class Column
```
## Properties
| Name | Description |
| --- | --- |
| [GroupLevel](../../aspose.cells/column/grouplevel/) { get; set; } | Gets the group level of the column. |
| [HasCustomStyle](../../aspose.cells/column/hascustomstyle/) { get; } | Indicates whether this column has custom style settings(different from the default one inherited from workbook). |
| [Index](../../aspose.cells/column/index/) { get; } | Gets the index of this column. |
| [IsCollapsed](../../aspose.cells/column/iscollapsed/) { get; set; } | whether the column is collapsed |
| [IsHidden](../../aspose.cells/column/ishidden/) { get; set; } | Indicates whether the column is hidden. |
| [Style](../../aspose.cells/column/style/) { get; } | (**Obsolete.**) Gets the style of this column. |
| [Width](../../aspose.cells/column/width/) { get; set; } | Gets and sets the column width in unit of characters. |
## Methods
| Name | Description |
| --- | --- |
| [ApplyStyle](../../aspose.cells/column/applystyle/)(Style, StyleFlag) | Applies formats for a whole column. |
| [GetStyle](../../aspose.cells/column/getstyle/)() | Gets the style of this column. |
| [SetStyle](../../aspose.cells/column/setstyle/)(Style) | Sets the style of this column. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class ColumnDemo
{
public static void ColumnExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add new Style to Workbook
Style style = workbook.CreateStyle();
// Setting the background color to Blue
style.BackgroundColor = Color.Blue;
// Setting the foreground color to Red
style.ForegroundColor = Color.Red;
// Setting Background Pattern
style.Pattern = BackgroundType.DiagonalStripe;
// New Style Flag
StyleFlag styleFlag = new StyleFlag();
// Set All Styles
styleFlag.All = true;
// Get first Column
Column column = worksheet.Cells.Columns[0];
// Apply Style to first Column
column.ApplyStyle(style, styleFlag);
// Setting additional properties
column.Width = 20.0; // Setting the column width
column.IsHidden = false; // Setting the column visibility
column.IsCollapsed = false; // Setting the column collapsed state
// Saving the Excel file
workbook.Save("ColumnExample.xlsx");
workbook.Save("ColumnExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
