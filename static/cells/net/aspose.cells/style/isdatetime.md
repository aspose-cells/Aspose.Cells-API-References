##Style.IsDateTime
Style property. Indicates whether the number format is a date format
## Style.IsDateTime property
Indicates whether the number format is a date format.
```csharp
public bool IsDateTime { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyIsDateTimeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Set a numeric value
cells["A1"].PutValue(1230);
// Get and modify the cell's style
Style style = cells["A1"].GetStyle();
// Set to date format (15 is the built-in date format)
style.Number = 15;
Console.WriteLine("IsDateTime after setting Number=15: " + style.IsDateTime);
// Set custom date format
style.Custom = "yyyy-mm-dd";
Console.WriteLine("IsDateTime after setting custom date format: " + style.IsDateTime);
// Apply the modified style back to the cell
cells["A1"].SetStyle(style);
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
