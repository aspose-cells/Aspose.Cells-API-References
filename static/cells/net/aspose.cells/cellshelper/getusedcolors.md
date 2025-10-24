##CellsHelper.GetUsedColors
CellsHelper method. Gets all used colors in the workbook
## CellsHelper.GetUsedColors method
Gets all used colors in the workbook.
```csharp
public static Color[] GetUsedColors(Workbook workbook)
```
| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The workbook object. |
### Return Value
The used colors.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class CellsHelperMethodGetUsedColorsWithWorkbookDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some colored cells to demonstrate used colors
worksheet.Cells["A1"].PutValue("Red Cell");
worksheet.Cells["A1"].GetStyle().ForegroundColor = Color.Red;
worksheet.Cells["A1"].GetStyle().Pattern = BackgroundType.Solid;
worksheet.Cells["A1"].SetStyle(worksheet.Cells["A1"].GetStyle());
worksheet.Cells["B1"].PutValue("Blue Cell");
worksheet.Cells["B1"].GetStyle().ForegroundColor = Color.Blue;
worksheet.Cells["B1"].GetStyle().Pattern = BackgroundType.Solid;
worksheet.Cells["B1"].SetStyle(worksheet.Cells["B1"].GetStyle());
worksheet.Cells["C1"].PutValue("Green Cell");
worksheet.Cells["C1"].GetStyle().ForegroundColor = Color.Green;
worksheet.Cells["C1"].GetStyle().Pattern = BackgroundType.Solid;
worksheet.Cells["C1"].SetStyle(worksheet.Cells["C1"].GetStyle());
try
{
// Call the GetUsedColors method with the workbook parameter
Color[] usedColors = CellsHelper.GetUsedColors(workbook);
// Display the used colors
Console.WriteLine("Used colors in the workbook:");
foreach (Color color in usedColors)
{
Console.WriteLine($"Color: A={color.A}, R={color.R}, G={color.G}, B={color.B}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetUsedColors method: {ex.Message}");
}
// Save the workbook
workbook.Save("CellsHelperGetUsedColorsDemo.xlsx");
}
}
}
```
### See Also
* class [Workbook](../../workbook/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
