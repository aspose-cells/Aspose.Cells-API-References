##Column.Style
Column property. Gets the style of this column
## Column.Style property
Gets the style of this column.
```csharp
[Obsolete("Use Column.GetStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style Style { get; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Column.GetStyle() method to get the default style of this column. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class ColumnPropertyStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the first column
Column column = worksheet.Cells.Columns[0];
// Get current style using Style property
Style originalStyle = column.Style;
Console.WriteLine("Original column style - Background: " + originalStyle.BackgroundColor);
// Create new style and modify properties
Style newStyle = workbook.CreateStyle();
newStyle.BackgroundColor = Color.LightBlue;
newStyle.Font.IsBold = true;
newStyle.HorizontalAlignment = TextAlignmentType.Center;
// Apply new style to the column
column.SetStyle(newStyle);
// Add data to demonstrate style application
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Data 1");
worksheet.Cells["A3"].PutValue("Data 2");
// Verify style changes
Console.WriteLine("New column style applied - Background: " + column.GetStyle().BackgroundColor);
// Save with column width adjustment
column.Width = 15;
workbook.Save("ColumnStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
