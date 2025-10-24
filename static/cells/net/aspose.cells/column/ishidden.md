##Column.IsHidden
Column property. Indicates whether the column is hidden
## Column.IsHidden property
Indicates whether the column is hidden.
```csharp
public bool IsHidden { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ColumnPropertyIsHiddenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set column width for demonstration
worksheet.Cells.Columns[1].Width = 20;
Console.WriteLine("Column 1 width before hiding: " + worksheet.Cells.Columns[1].Width);
// Hide the column
worksheet.Cells.Columns[1].IsHidden = true;
Console.WriteLine("Column 1 is hidden: " + worksheet.Cells.Columns[1].IsHidden);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
