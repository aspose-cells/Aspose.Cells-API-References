##Timeline.TopPixel
Timeline property. Returns or sets the vertical offset of timeline shape from its top row in pixels
## Timeline.TopPixel property
Returns or sets the vertical offset of timeline shape from its top row, in pixels.
```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;
namespace AsposeCellsExamples
{
public class TimelinePropertyTopPixelDemo
{
public static void Run()
{
// Create a new workbook and get the first worksheet
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
// Populate sample data
cells["A1"].Value = "Date";
cells["A2"].Value = new DateTime(2023, 1, 1);
cells["A3"].Value = new DateTime(2023, 2, 1);
cells["A4"].Value = new DateTime(2023, 3, 1);
cells["B1"].Value = "Sales";
cells["B2"].Value = 1000;
cells["B3"].Value = 2000;
cells["B4"].Value = 3000;
// Add PivotTable
int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "Date");
pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
pivot.RefreshData();
pivot.CalculateData();
// Add Timeline
int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
Timeline timeline = sheet.Timelines[timelineIndex];
// Set Timeline properties including TopPixel
timeline.TopPixel = 50;
timeline.HeightPixel = 100;
timeline.WidthPixel = 300;
// Save the workbook
book.Save("TimelineTopPixelDemo.xlsx");
}
}
}
```
### See Also
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
