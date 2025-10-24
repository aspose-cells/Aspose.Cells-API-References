##AutoFitterOptions.MaxRowHeight
AutoFitterOptions property. Gets and sets the max row heightin unit of Point when autofitting rows
## AutoFitterOptions.MaxRowHeight property
Gets and sets the max row height(in unit of Point) when autofitting rows.
```csharp
public double MaxRowHeight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFitterOptionsPropertyMaxRowHeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data and formatting
worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row auto-fitting");
Style style = worksheet.Cells["A1"].GetStyle();
style.IsTextWrapped = true;
worksheet.Cells["A1"].SetStyle(style);
worksheet.Cells.SetRowHeight(0, 10); // Set initial small row height
// Create AutoFitterOptions with MaxRowHeight setting
AutoFitterOptions options = new AutoFitterOptions
{
MaxRowHeight = 50, // Limit maximum row height to 50 pixels
OnlyAuto = true
};
// Auto-fit the row with height limitation
worksheet.AutoFitRows(0, 0, options);
Console.WriteLine("Row height after auto-fit with MaxRowHeight=50: " + worksheet.Cells.GetRowHeight(0));
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
