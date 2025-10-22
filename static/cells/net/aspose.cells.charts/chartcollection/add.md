##ChartCollection.Add
ChartCollection method. Adds a chart to the collection
## Add(ChartType, int, int, int, int) {#add}
Adds a chart to the collection.
```csharp
public int Add(ChartType type, int upperLeftRow, int upperLeftColumn, int lowerRightRow,
int lowerRightColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| lowerRightRow | Int32 | Lower right row index |
| lowerRightColumn | Int32 | Lower right column index |
### Return Value
[`Chart`](../../chart/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartCollectionMethodAddWithChartTypeInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for the chart
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["B1"].PutValue("Value");
for (int i = 1; i <= 10; i++)
{
sheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
sheet.Cells["B" + (i + 1)].PutValue(i * 10);
}
// Add a chart using the specified parameters
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 2, 25, 11);
Chart chart = sheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("=Sheet1!$A$1:$B$11", true);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## Add(ChartType, string, int, int, int, int) {#add_2}
Adds a chart to the collection.
```csharp
[Obsolete("Use ChartCollection.Add(ChartType, string, bool ,int , int, int, int ) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ChartType type, string dataRange, int topRow, int leftColumn, int rightRow,
int bottomColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| dataRange | String | Specifies the data range of the chart |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| rightRow | Int32 | Lower right row index |
| bottomColumn | Int32 | Lower right column index |
### Return Value
[`Chart`](../../chart/) object index.
### Remarks
NOTE: This member is now obsolete. Instead, please use `Add` property. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartCollectionMethodAddWithChartTypeStringInt32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
try
{
// Call the Add method with parameters (ChartType, String, Int32, Int32, Int32, Int32)
int chartIndex = worksheet.Charts.Add(
ChartType.Column,          // Chart type
"A1:B4",                  // Data range
0,                        // Top row position
3,                        // Left column position
15,                       // Bottom row position
8                         // Right column position
);
Console.WriteLine("Chart added successfully at index: " + chartIndex);
// Access the newly created chart
Chart chart = worksheet.Charts[chartIndex];
chart.Title.Text = "Sample Column Chart";
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("ChartCollectionMethodAddDemo.xlsx");
}
}
}
```
### See Also
* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## Add(byte[], string, bool, int, int, int, int) {#add_3}
Adds a chart with preset template.
```csharp
public int Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn,
int rightRow, int bottomColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| data | Byte[] | The data of chart template file(.crtx). |
| dataRange | String | Specifies the data range of the chart |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| rightRow | Int32 | Lower right row index |
| bottomColumn | Int32 | Lower right column index |
### Return Value
[`Chart`](../../chart/) object index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartCollectionMethodAddWithByteArrayStringBooleanInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Create a byte array representing chart data (simplified example)
byte[] chartData = new byte[] { 0x01, 0x02, 0x03 };
try
{
// Call the Add method with specific parameters
int chartIndex = worksheet.Charts.Add(
chartData,          // Byte[] data
"A1:B4",            // String dataRange
true,               // Boolean isVertical
0,                  // Int32 topRow
0,                  // Int32 leftColumn
15,                 // Int32 rightRow
8                   // Int32 bottomColumn
);
Console.WriteLine($"Chart added successfully at index: {chartIndex}");
// Access the added chart
Chart chart = worksheet.Charts[chartIndex];
chart.Type = ChartType.Column;
// Save the result
workbook.Save("ChartCollectionMethodAddDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
}
}
}
```
### See Also
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## Add(ChartType, string, bool, int, int, int, int) {#add_1}
Adds a chart to the collection.
```csharp
public int Add(ChartType type, string dataRange, bool isVertical, int topRow, int leftColumn,
int rightRow, int bottomColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| dataRange | String | Specifies the data range of the chart |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| rightRow | Int32 | Lower right row index |
| bottomColumn | Int32 | Lower right column index |
### Return Value
[`Chart`](../../chart/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartCollectionMethodAddWithChartTypeStringBooleanInt32IntDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Series1");
worksheet.Cells["C1"].PutValue("Series2");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["C2"].PutValue(20);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(30);
worksheet.Cells["C3"].PutValue(40);
// Add chart with specified parameters
int chartIndex = worksheet.Charts.Add(ChartType.Column, "A1:C3", true, 4, 4, 14, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
