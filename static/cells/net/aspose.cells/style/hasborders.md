##Style.HasBorders
Style property. Checks whether there are borders have been set for the style
## Style.HasBorders property
Checks whether there are borders have been set for the style.
```csharp
public bool HasBorders { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyHasBordersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Access cell A1 and check if it has borders (should be false by default)
Cell cellA1 = cells["A1"];
Console.WriteLine("Cell A1 has borders: " + cellA1.GetStyle().HasBorders);
// Create a style with borders
Style styleWithBorders = workbook.CreateStyle();
styleWithBorders.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
styleWithBorders.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
// Apply the style to cell B1
Cell cellB1 = cells["B1"];
cellB1.SetStyle(styleWithBorders);
// Check if cell B1 has borders (should be true now)
Console.WriteLine("Cell B1 has borders: " + cellB1.GetStyle().HasBorders);
// Save the workbook
workbook.Save("HasBordersDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
