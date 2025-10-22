##Column.IsCollapsed
Column property. whether the column is collapsed
## Column.IsCollapsed property
whether the column is collapsed
```csharp
public bool IsCollapsed { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ColumnPropertyIsCollapsedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create and apply a simple style to the column
Style style = workbook.CreateStyle();
style.BackgroundColor = Color.LightGray;
Column column = worksheet.Cells.Columns[0];
column.ApplyStyle(style, new StyleFlag { All = true });
// Set column properties including IsCollapsed
column.Width = 15;
column.IsCollapsed = true; // Demonstrating IsCollapsed property
column.IsHidden = false;
// Add some data to visualize the collapsed column
worksheet.Cells["A1"].PutValue("Collapsed Column");
worksheet.Cells["B1"].PutValue("Visible Column");
workbook.Save("ColumnIsCollapsedDemo.xlsx");
}
}
}
```
### See Also
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
