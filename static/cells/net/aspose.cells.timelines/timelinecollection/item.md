##TimelineCollection.Item
TimelineCollection property. Gets the Timeline by index
## TimelineCollection indexer (1 of 2)
Gets the Timeline by index.
```csharp
public Timeline this[int index] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class TimelineCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].PutValue("Date");
sheet.Cells["A2"].PutValue(DateTime.Now);
sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
// Create pivot table first
int pivotIndex = sheet.PivotTables.Add("A1:A3", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add timeline to the worksheet
int index = sheet.Timelines.Add(pivotTable, 0, 0, "Date");
// Access timeline using Item property by index
Timeline timelineByIndex = sheet.Timelines[index];
// Demonstrate usage of the timeline
Console.WriteLine("Timeline name: " + timelineByIndex.Name);
}
}
}
```
### See Also
* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
## TimelineCollection indexer (2 of 2)
Gets the Timeline by Timeline's name.
```csharp
public Timeline this[string name] { get; }
```
### Examples
```csharp
[C#]
//Get the Timeline by Timeline's name.
Timeline objByName = sheet.Timelines["date"];
```
### See Also
* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
