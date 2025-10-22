##Timeline.WidthPixel
Timeline property. Returns or sets the width of the specified timeline in pixels
## Timeline.WidthPixel property
Returns or sets the width of the specified timeline, in pixels.
```csharp
[Obsolete("Use Shape.Width property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int WidthPixel { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Width property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;
namespace AsposeCellsExamples
{
public class TimelinePropertyWidthPixelDemo
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
sheet.Cells["A4"].Value = new DateTime(2023, 3, 1);
sheet.Cells["B1"].Value = "Sales";
sheet.Cells["B2"].Value = 1000;
sheet.Cells["B3"].Value = 2000;
sheet.Cells["B4"].Value = 3000;
// Create pivot table and get the reference
int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "Date");
pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
pivot.RefreshData();
pivot.CalculateData();
// Add timeline and get the reference
int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
Timeline timeline = sheet.Timelines[timelineIndex];
// Set timeline properties including WidthPixel
timeline.WidthPixel = 300;
timeline.HeightPixel = 100;
timeline.Caption = "Sales Timeline";
// Save the workbook
workbook.Save("TimelineWidthPixelDemo.xlsx");
}
}
}
```
### See Also
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
