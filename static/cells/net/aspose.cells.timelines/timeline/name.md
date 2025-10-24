##Timeline.Name
Timeline property. Returns or sets the name of the specified Timeline
## Timeline.Name property
Returns or sets the name of the specified Timeline
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class TimelinePropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for the timeline
sheet.Cells["A1"].PutValue("Date");
sheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
sheet.Cells["A3"].PutValue(DateTime.Now);
sheet.Cells["A4"].PutValue(DateTime.Now.AddDays(1));
// Add a pivot table that will be used as data source for timeline
sheet.Cells["C1"].PutValue("Pivot Table");
int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add a timeline using the pivot table
int timelineIndex = sheet.Timelines.Add(pivotTable, 0, 0, "Timeline1");
Aspose.Cells.Timelines.Timeline timeline = sheet.Timelines[timelineIndex];
// Set and demonstrate the Name property
timeline.Name = "MyTimeline";
Console.WriteLine("Timeline name: " + timeline.Name);
}
}
}
```
### See Also
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
