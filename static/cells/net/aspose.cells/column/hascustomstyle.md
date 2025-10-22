##Column.HasCustomStyle
Column property. Indicates whether this column has custom style settingsdifferent from the default one inherited from workbook
## Column.HasCustomStyle property
Indicates whether this column has custom style settings(different from the default one inherited from workbook).
```csharp
public bool HasCustomStyle { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class ColumnPropertyHasCustomStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the first column
Column column = worksheet.Cells.Columns[0];
// Display initial HasCustomState value
Console.WriteLine("Initial HasCustomStyle: " + column.HasCustomStyle);
// Modify column style to demonstrate HasCustomStyle change
Style columnStyle = column.GetStyle();
columnStyle.BackgroundColor = Color.LightBlue;
column.SetStyle(columnStyle);
// Display updated HasCustomStyle value
Console.WriteLine("After style modification - HasCustomStyle: " + column.HasCustomStyle);
// Create another column with default style for comparison
Column secondColumn = worksheet.Cells.Columns[1];
Console.WriteLine("Second column HasCustomStyle: " + secondColumn.HasCustomStyle);
// Save the workbook
workbook.Save("ColumnHasCustomStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
