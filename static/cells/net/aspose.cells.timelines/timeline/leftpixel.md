##Timeline.LeftPixel
Timeline property. Returns or sets the horizontal offset of timeline shape from its left column in pixels
## Timeline.LeftPixel property
Returns or sets the horizontal offset of timeline shape from its left column, in pixels.
```csharp
[Obsolete("Use Shape.Left property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int LeftPixel { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;
namespace AsposeCellsExamples
{
public class TimelinePropertyLeftPixelDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].Value = "Date";
sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
sheet.Cells["A3"].Value = new DateTime(2023, 2, 1);
sheet.Cells["B1"].Value = "Sales";
sheet.Cells["B2"].Value = 1000;
sheet.Cells["B3"].Value = 2000;
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "Date");
pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
pivot.RefreshData();
// Add timeline and get it from the collection
int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
Timeline timeline = sheet.Timelines[timelineIndex];
// Demonstrate LeftPixel property
timeline.LeftPixel = 150;
timeline.TopPixel = 50;
timeline.WidthPixel = 200;
timeline.HeightPixel = 80;
// Save workbook
workbook.Save("TimelineLeftPixelDemo.xlsx");
}
}
}
```
### See Also
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
