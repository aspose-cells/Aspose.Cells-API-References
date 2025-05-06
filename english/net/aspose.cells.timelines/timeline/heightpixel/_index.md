---
title: Timeline.HeightPixel
second_title: Aspose.Cells for .NET API Reference
description: Timeline property. Returns or sets the height of the specified timeline in pixels
type: docs
url: /net/aspose.cells.timelines/timeline/heightpixel/
---
## Timeline.HeightPixel property

Returns or sets the height of the specified timeline, in pixels.

```csharp
public int HeightPixel { get; set; }
```

### Examples

```csharp
// Called: timelineObj.HeightPixel = 100;
public static void Property_HeightPixel()
        {
            // Create a new workbook and get the first worksheet
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate the worksheet with sample data
            cells[0, 0].Value = &quot;fruit&quot;;
            cells[1, 0].Value = &quot;grape&quot;;
            cells[2, 0].Value = &quot;blueberry&quot;;
            cells[3, 0].Value = &quot;kiwi&quot;;
            cells[4, 0].Value = &quot;cherry&quot;;

            // Create date style
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = &quot;m/d/yyyy&quot;;
            cells[0, 1].Value = &quot;date&quot;;
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);
            // Set date style
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = &quot;amount&quot;;
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // Add a PivotTable
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add(&quot;=Sheet1!A1:C5&quot;, &quot;A12&quot;, &quot;TestPivotTable&quot;);
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, &quot;fruit&quot;);
            pivot.AddFieldToArea(PivotFieldType.Column, &quot;date&quot;);
            pivot.AddFieldToArea(PivotFieldType.Data, &quot;amount&quot;);
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Refresh PivotTable data
            pivot.RefreshData();
            pivot.CalculateData();

            // Add a new Timeline using PivotTable as data source
            sheet.Timelines.Add(pivot, 10, 5, &quot;date&quot;);

            // Get Timeline object
            Timeline timelineObj = sheet.Timelines[0];

            // Set properties of the Timeline
            timelineObj.Caption = &quot;timeline caption test&quot;;
            timelineObj.Name = &quot;timeline name test&quot;;
            timelineObj.LeftPixel = 100;
            timelineObj.TopPixel = 50;
            timelineObj.WidthPixel = 300;
            timelineObj.HeightPixel = 100;

            // Save the workbook
            book.Save(&quot;TimelineExample.xlsx&quot;);
        }
```

### See Also

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


