##Style.ToJson
Style method. Convert Style to JSON struct data
## Style.ToJson method
Convert [`Style`](../) to JSON struct data.
```csharp
public string ToJson()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleMethodToJsonDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create and apply a style to cell B4
Style style = workbook.CreateStyle();
style.BackgroundColor = System.Drawing.Color.Yellow;
cells["B4"].SetStyle(style);
// Convert style to JSON
string styleJson = style.ToJson();
Console.WriteLine("Style JSON:");
Console.WriteLine(styleJson);
// Set formula in cell B6
cells["B6"].Formula = "=A1";
// Convert cell to JSON
string cellJson = cells["B6"].ToJson();
Console.WriteLine("\nCell JSON:");
Console.WriteLine(cellJson);
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
