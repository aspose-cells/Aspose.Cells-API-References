##DataSorter.AddColorKey
DataSorter method. Adds color sort key
## DataSorter.AddColorKey method
Adds color sort key.
```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```
| Parameter | Type | Description |
| --- | --- | --- |
| key | Int32 | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | SortOnType | The sorted color value type. |
| order | SortOrder | The sort order. |
| color | Color | The custom sort color. |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataSorterMethodAddColorKeyWithInt32SortOnTypeSortOrderColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with colored cells
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue(5);
worksheet.Cells["A3"].PutValue(3);
worksheet.Cells["A4"].PutValue(7);
// Apply colors to cells
Style styleRed = workbook.CreateStyle();
styleRed.ForegroundColor = Color.Red;
styleRed.Pattern = BackgroundType.Solid;
worksheet.Cells["A2"].SetStyle(styleRed);
Style styleBlue = workbook.CreateStyle();
styleBlue.ForegroundColor = Color.Blue;
styleBlue.Pattern = BackgroundType.Solid;
worksheet.Cells["A3"].SetStyle(styleBlue);
Style styleGreen = workbook.CreateStyle();
styleGreen.ForegroundColor = Color.Green;
styleGreen.Pattern = BackgroundType.Solid;
worksheet.Cells["A4"].SetStyle(styleGreen);
// Create data sorter and add color key
DataSorter sorter = workbook.DataSorter;
sorter.HasHeaders = true;
sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);
// Sort the data
sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A4"));
// Output the sorted values (for demonstration)
Console.WriteLine("Sorted values:");
for (int i = 1; i <= 3; i++)
{
Console.WriteLine(worksheet.Cells["A" + (i + 1)].IntValue);
}
}
}
}
```
### See Also
* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
