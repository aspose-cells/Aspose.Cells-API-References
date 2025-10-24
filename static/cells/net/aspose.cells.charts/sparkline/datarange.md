##Sparkline.DataRange
Sparkline property. Represents the data range of the sparkline
## Sparkline.DataRange property
Represents the data range of the sparkline.
```csharp
public string DataRange { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklinePropertyDataRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(5);
sheet.Cells["A2"].PutValue(3);
sheet.Cells["A3"].PutValue(7);
sheet.Cells["A4"].PutValue(2);
sheet.Cells["A5"].PutValue(9);
// Add a sparkline group
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A5", false, new CellArea { StartRow = 0, StartColumn = 1, EndRow = 0, EndColumn = 1 });
SparklineGroup group = sheet.SparklineGroups[idx];
// Access the first sparkline and display its data range
Sparkline sparkline = group.Sparklines[0];
Console.WriteLine("Sparkline DataRange: " + sparkline.DataRange);
}
}
}
```
### See Also
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
