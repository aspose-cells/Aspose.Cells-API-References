##Row.Item
Row property. Gets the cell
## Row indexer
Gets the cell.
```csharp
public Cell this[int column] { get; }
```
| Parameter | Description |
| --- | --- |
| column | The column index |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Access the first row
Row row = sheet.Cells.Rows[0];
// Set HTML content with different color styles
row[0].HtmlString = @"<span style=""color:#ffAb68;"">TEST</span>";
row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
// Demonstrate Item property usage and output the colors
Console.WriteLine("Cell 0 Font Color: " + row[0].GetStyle().Font.Color.Name);
Console.WriteLine("Cell 1 Font Color: " + row[1].GetStyle().Font.Color.Name);
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
