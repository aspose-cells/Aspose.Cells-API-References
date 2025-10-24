##Range.Item
Range property. Gets Cell object in this range
## Range indexer
Gets [`Cell`](../../cell/) object in this range.
```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```
| Parameter | Description |
| --- | --- |
| rowOffset | Row offset in this range, zero based. |
| columnOffset | Column offset in this range, zero based. |
### Return Value
[`Cell`](../../cell/) object.
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RangePropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
DataTable dt = new DataTable();
dt.Columns.Add("Id", typeof(int));
dt.Columns.Add("Name", typeof(string));
dt.Rows.Add(1001, "Item 1");
dt.Rows.Add(1002, "Item 2");
// Create a range and demonstrate Item property
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B3");
// Set headers using Item property
range[0, 0].PutValue("Id");
range[0, 1].PutValue("Name");
// Fill data using Item property
for (int i = 0; i < dt.Rows.Count; i++)
{
range[i + 1, 0].PutValue(dt.Rows[i]["Id"]);
range[i + 1, 1].PutValue(dt.Rows[i]["Name"]);
}
// Format header row using Item property
Style style = workbook.CreateStyle();
style.ForegroundColor = Color.FromArgb(0, 176, 80);
range[0, 0].SetStyle(style);
range[0, 1].SetStyle(style);
// Save the workbook
workbook.Save("RangePropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
