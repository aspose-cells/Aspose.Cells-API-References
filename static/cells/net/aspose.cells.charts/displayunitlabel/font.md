##DisplayUnitLabel.Font
DisplayUnitLabel property. Gets a Font object of the specified ChartFrame object
## DisplayUnitLabel.Font property
Gets a `Font` object of the specified ChartFrame object.
```csharp
public override Font Font { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class DisplayUnitLabelPropertyFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue(1000);
worksheet.Cells["A2"].PutValue(2000);
worksheet.Cells["A3"].PutValue(3000);
worksheet.Cells["A4"].PutValue(4000);
worksheet.Cells["A5"].PutValue(5000);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A5", true);
// Set display units for value axis
chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
chart.ValueAxis.DisplayUnitLabel.Text = "Thousands";
// Get the DisplayUnitLabel instance
DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
// Display current font properties
Font currentFont = displayUnitLabel.Font;
Console.WriteLine("Current Font Properties:");
Console.WriteLine($"Name: {currentFont.Name}");
Console.WriteLine($"Size: {currentFont.Size}");
Console.WriteLine($"Color: {currentFont.Color}");
Console.WriteLine($"Bold: {currentFont.IsBold}");
Console.WriteLine($"Italic: {currentFont.IsItalic}");
// Create a new font style and apply it to the display unit label
// Note: Since Font is read-only, we modify its properties directly
currentFont.Name = "Arial";
currentFont.Size = 12;
currentFont.Color = System.Drawing.Color.Red;
currentFont.IsBold = true;
currentFont.IsItalic = false;
currentFont.Underline = FontUnderlineType.Single;
// Save the workbook to see the changes
workbook.Save("DisplayUnitLabelFontDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../../../aspose.cells/font/)
* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
