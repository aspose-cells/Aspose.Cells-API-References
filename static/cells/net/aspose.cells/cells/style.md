##Cells.Style
Cells property. Gets and sets the default style of the worksheet
## Cells.Style property
Gets and sets the default style of the worksheet.
```csharp
public Style Style { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set a value in cell A1
Cell cell = cells["A1"];
cell.PutValue(43368); // This represents the date 2018-09-25
// Get the default style and modify its format
Style style = cells.Style;
style.CultureCustom = "yyyymmdd!y";
// Apply the modified style to the cell
cell.SetStyle(style);
// Display the formatted string value
Console.WriteLine("Formatted value: " + cell.StringValue);
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
