##Range.CurrentRegion
Range property. Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns
## Range.CurrentRegion property
Returns a Range object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns.
```csharp
public Range CurrentRegion { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class RangePropertyCurrentRegionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate data with some blank cells to create regions
worksheet.Cells["A1"].PutValue("Region 1");
worksheet.Cells["A2"].PutValue("Data 1");
worksheet.Cells["A3"].PutValue("Data 2");
worksheet.Cells["A4"].PutValue("Data 3");
// Leave row 5 blank to separate regions
worksheet.Cells["A6"].PutValue("Region 2");
worksheet.Cells["A7"].PutValue("Data 4");
worksheet.Cells["B7"].PutValue("Data 5");
worksheet.Cells["A8"].PutValue("Data 6");
// Get a cell in the first region and convert to Range
Aspose.Cells.Range cellInRegion1 = worksheet.Cells.CreateRange("A2", "A2");
Aspose.Cells.Range currentRegion1 = cellInRegion1.CurrentRegion;
Console.WriteLine("CurrentRegion for A2: " + currentRegion1.Address);
Console.WriteLine("Row count in region: " + currentRegion1.RowCount);
Console.WriteLine("Column count in region: " + currentRegion1.ColumnCount);
// Get a cell in the second region and convert to Range
Aspose.Cells.Range cellInRegion2 = worksheet.Cells.CreateRange("B7", "B7");
Aspose.Cells.Range currentRegion2 = cellInRegion2.CurrentRegion;
Console.WriteLine("\nCurrentRegion for B7: " + currentRegion2.Address);
Console.WriteLine("Row count in region: " + currentRegion2.RowCount);
Console.WriteLine("Column count in region: " + currentRegion2.ColumnCount);
// Apply formatting to the entire current region
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.LightBlue;
style.Pattern = BackgroundType.Solid;
currentRegion1.SetStyle(style);
// Save the workbook
workbook.Save("RangePropertyCurrentRegionDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
