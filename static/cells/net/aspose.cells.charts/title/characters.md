##Title.Characters
Title method. Gets rich text formatting of this Title
## Title.Characters method
Gets rich text formatting of this Title.
```csharp
public FontSetting[] Characters()
```
### Return Value
returns FontSetting array
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class TitleMethodCharactersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to worksheet
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["A2"].PutValue("Apples");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("Oranges");
worksheet.Cells["B3"].PutValue(5);
// Create a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Set chart title
chart.Title.Text = "Fruit Sales Report";
chart.Title.IsVisible = true;
try
{
// Get the rich text formatting of the title
FontSetting[] titleCharacters = chart.Title.Characters();
// Modify the first character's font
if (titleCharacters.Length > 0)
{
titleCharacters[0].Font.Color = System.Drawing.Color.Red;
titleCharacters[0].Font.IsBold = true;
titleCharacters[0].Font.Size = 14;
}
Console.WriteLine("Characters method executed successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Characters method: {ex.Message}");
}
// Save the result
workbook.Save("TitleMethodCharactersDemo.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
