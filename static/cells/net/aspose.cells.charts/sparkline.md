##Class Sparkline
Aspose.Cells.Charts.Sparkline class. A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data
## Sparkline class
A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.
```csharp
public class Sparkline
```
## Properties
| Name | Description |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column/) { get; } | Gets the column index of the sparkline. |
| [DataRange](../../aspose.cells.charts/sparkline/datarange/) { get; set; } | Represents the data range of the sparkline. |
| [Row](../../aspose.cells.charts/sparkline/row/) { get; } | Gets the row index of the sparkline. |
## Methods
| Name | Description |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage)(ImageOrPrintOptions) | Converts a sparkline to an image. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_1)(Stream, ImageOrPrintOptions) | Converts a sparkline to an image. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_2)(string, ImageOrPrintOptions) | Converts a sparkline to an image. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Rendering;
using System;
using System.IO;
public class SparklineDemo
{
public static void SparklineExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some data to the worksheet
sheet.Cells["A1"].PutValue(5);
sheet.Cells["B1"].PutValue(2);
sheet.Cells["C1"].PutValue(1);
sheet.Cells["D1"].PutValue(3);
// Define the CellArea for the sparkline
CellArea ca = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
// Add a sparkline group to the worksheet
int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Add a sparkline to the group
idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);
Sparkline line = group.Sparklines[idx];
// Output sparkline details
Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);
// Save the sparkline as an image
ImageOrPrintOptions options = new ImageOrPrintOptions
{
ImageType = Aspose.Cells.Drawing.ImageType.Png,
HorizontalResolution = 300,
VerticalResolution = 300
};
line.ToImage("output.png", options);
// Save the workbook
workbook.Save("SparklineExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
