##Class Timeline
Aspose.Cells.Timelines.Timeline class. Summary description of Timeline View Due to MS Excel Excel 2003 does not support Timeline
## Timeline class
Summary description of Timeline View Due to MS Excel, Excel 2003 does not support Timeline
```csharp
public class Timeline
```
## Properties
| Name | Description |
| --- | --- |
| [Caption](../../aspose.cells.timelines/timeline/caption/) { get; set; } | Returns or sets the caption of the specified Timeline. |
| [HeightPixel](../../aspose.cells.timelines/timeline/heightpixel/) { get; set; } | (**Obsolete.**) Returns or sets the height of the specified timeline, in pixels. |
| [LeftPixel](../../aspose.cells.timelines/timeline/leftpixel/) { get; set; } | (**Obsolete.**) Returns or sets the horizontal offset of timeline shape from its left column, in pixels. |
| [Name](../../aspose.cells.timelines/timeline/name/) { get; set; } | Returns or sets the name of the specified Timeline |
| [Shape](../../aspose.cells.timelines/timeline/shape/) { get; } | Returns the [`TimelineShape`](../../aspose.cells.drawing/timelineshape/) object associated with this Timeline. Read-only. |
| [TopPixel](../../aspose.cells.timelines/timeline/toppixel/) { get; set; } | (**Obsolete.**) Returns or sets the vertical offset of timeline shape from its top row, in pixels. |
| [WidthPixel](../../aspose.cells.timelines/timeline/widthpixel/) { get; set; } | (**Obsolete.**) Returns or sets the width of the specified timeline, in pixels. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;
using System;
public class TimelineDemo
{
public static void TimelineExample()
{
// Create a new workbook and get the first worksheet
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
// Populate the worksheet with sample data
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
// Create date style
Style dateStyle = new CellsFactory().CreateStyle();
dateStyle.Custom = "m/d/yyyy";
cells[0, 1].Value = "date";
cells[1, 1].Value = new DateTime(2021, 2, 5);
cells[2, 1].Value = new DateTime(2022, 3, 8);
cells[3, 1].Value = new DateTime(2023, 4, 10);
cells[4, 1].Value = new DateTime(2024, 5, 16);
// Set date style
cells[1, 1].SetStyle(dateStyle);
cells[2, 1].SetStyle(dateStyle);
cells[3, 1].SetStyle(dateStyle);
cells[4, 1].SetStyle(dateStyle);
cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
// Add a PivotTable
PivotTableCollection pivots = sheet.PivotTables;
int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "date");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
// Refresh PivotTable data
pivot.RefreshData();
pivot.CalculateData();
// Add a new Timeline using PivotTable as data source
sheet.Timelines.Add(pivot, 10, 5, "date");
// Get Timeline object
Timeline timelineObj = sheet.Timelines[0];
// Set properties of the Timeline
timelineObj.Caption = "timeline caption test";
timelineObj.Name = "timeline name test";
timelineObj.LeftPixel = 100;
timelineObj.TopPixel = 50;
timelineObj.WidthPixel = 300;
timelineObj.HeightPixel = 100;
// Save the workbook
book.Save("TimelineExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Timelines](../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../)
