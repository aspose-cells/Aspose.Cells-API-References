##SparklineGroupCollection.Add
SparklineGroupCollection method. Adds an SparklineGroup with a Sparkline to the collection
## Add(SparklineType) {#add}
Adds an [`SparklineGroup`](../../sparklinegroup/) with a [`Sparkline`](../../sparkline/) to the collection.
```csharp
public int Add(SparklineType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | SparklineType | Specifies the type of the Sparkline group. |
### Return Value
[`SparklineGroup`](../../sparklinegroup/) object index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class SparklineGroupCollectionMethodAddWithSparklineTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for sparklines
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["A2"].PutValue(3);
worksheet.Cells["A3"].PutValue(7);
worksheet.Cells["A4"].PutValue(2);
worksheet.Cells["A5"].PutValue(9);
try
{
// Get the sparkline group collection
SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;
// Call the Add method with SparklineType parameter
int index = sparklineGroups.Add(SparklineType.Line);
// Configure the sparkline group
SparklineGroup group = sparklineGroups[index];
group.Sparklines.Add("A1:A5", 5, 0);
Console.WriteLine("Sparkline group added successfully with type: Line");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("SparklineGroupCollectionMethodAddWithSparklineTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## Add(SparklineType, string, bool, CellArea) {#add_1}
Adds an [`SparklineGroup`](../../sparklinegroup/) with [`Sparkline`](../../sparkline/) to the collection.
```csharp
public int Add(SparklineType type, string dataRange, bool isVertical, CellArea locationRange)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | SparklineType | Specifies the type of the Sparkline group. |
| dataRange | String | Specifies the data range of the sparkline group. |
| isVertical | Boolean | Specifies whether to plot the sparklines from the data range by row or by column. |
| locationRange | CellArea | Specifies where the sparklines to be placed. |
### Return Value
[`SparklineGroup`](../../sparklinegroup/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupCollectionMethodAddWithSparklineTypeStringBooleanCellDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for sparklines
sheet.Cells["A1"].PutValue(5);
sheet.Cells["B1"].PutValue(3);
sheet.Cells["C1"].PutValue(8);
// Add sparkline group with specified parameters
sheet.SparklineGroups.Add(
SparklineType.Line,
"A1:C1",
false,
CellArea.CreateCellArea("D1", "D1")
);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [SparklineType](../../sparklinetype/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
