##PivotTableFormat.GetStyle
PivotTableFormat method. Gets the formatted style
## PivotTableFormat.GetStyle method
Gets the formatted style.
```csharp
public Style GetStyle()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableFormatMethodGetStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 2000;
worksheet.Cells["B4"].Value = 3000;
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Get pivot table format
PivotTableFormatCollection formats = pivotTable.PivotFormats;
PivotTableFormat format = formats[0];
try
{
// Call the GetStyle method
Style style = format.GetStyle();
// Display style properties
Console.WriteLine("Style properties:");
Console.WriteLine($"Font Name: {style.Font.Name}");
Console.WriteLine($"Font Size: {style.Font.Size}");
Console.WriteLine($"Background Color: {style.BackgroundColor}");
// Modify the style
style.Font.Name = "Arial";
style.Font.Size = 12;
style.BackgroundColor = System.Drawing.Color.LightBlue;
// Apply the modified style back to the format
format.SetStyle(style);
Console.WriteLine("GetStyle method executed successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetStyle method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableFormatMethodGetStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
