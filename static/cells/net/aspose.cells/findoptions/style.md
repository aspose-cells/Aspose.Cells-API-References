##FindOptions.Style
FindOptions property. The format to search for
## FindOptions.Style property
The format to search for.
```csharp
public Style Style { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsPropertyStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with blue font
Style style = workbook.CreateStyle();
style.Font.Color = System.Drawing.Color.Blue;
// Apply the style to cell F2
Cell cell = worksheet.Cells["F2"];
cell.PutValue("SearchTarget");
cell.SetStyle(style);
// Create find options with the style
FindOptions options = new FindOptions();
options.Style = style;
// Find cell with matching style
Cell foundCell = worksheet.Cells.Find(null, null, options);
// Output the found cell's name
Console.WriteLine("Cell found with matching style: " + foundCell?.Name);
}
}
}
```
### See Also
* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
