##SparklineCollection.Add
SparklineCollection method. Add a sparkline
## SparklineCollection.Add method
Add a sparkline.
```csharp
public int Add(string dataRange, int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | String | Specifies the new data range of the sparkline. |
| row | Int32 | The row index of the location. |
| column | Int32 | The column index of the location. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineCollectionMethodAddWithStringInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
for (int i = 0; i < 12; i++)
{
worksheet.Cells[4, 3 + i].PutValue(i + 1);
}
// Create a sparkline group
int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
SparklineGroup group = worksheet.SparklineGroups[groupIndex];
// Add sparkline with data range and location
int sparklineIndex = group.Sparklines.Add("D5:O5", 4, 15);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
