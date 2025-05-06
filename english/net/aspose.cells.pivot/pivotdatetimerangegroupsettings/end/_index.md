---
title: PivotDateTimeRangeGroupSettings.End
second_title: Aspose.Cells for .NET API Reference
description: PivotDateTimeRangeGroupSettings property. Gets the end date time of the group
type: docs
url: /net/aspose.cells.pivot/pivotdatetimerangegroupsettings/end/
---
## PivotDateTimeRangeGroupSettings.End property

Gets the end date time of the group.

```csharp
public DateTime End { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;End Date: &amp;quot; + groupSettings.End);
public static void Property_End()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Date&quot;);
            Style style = workbook.CreateStyle();
            style.Number = 14;//m/d/yyy
            worksheet.Cells[&quot;A2&quot;].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells[&quot;A2&quot;].SetStyle(style);

            worksheet.Cells[&quot;A3&quot;].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells[&quot;A3&quot;].SetStyle(style);

            worksheet.Cells[&quot;A4&quot;].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells[&quot;A4&quot;].SetStyle(style);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add(&quot;=A1:B4&quot;, &quot;E3&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value field

            //TODO
            PivotField dateField = pivotTable.RowFields[0];

            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // Access the group settings
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

            // Output the group settings
            Console.WriteLine(&quot;Group Type: &quot; + groupSettings.Type);
            Console.WriteLine(&quot;Start Date: &quot; + groupSettings.Start);
            Console.WriteLine(&quot;End Date: &quot; + groupSettings.End);
            Console.WriteLine(&quot;Interval: &quot; + groupSettings.Interval);
            Console.WriteLine(&quot;Is Grouped By Months: &quot; + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // Save the workbook
            workbook.Save(&quot;PivotGroupByTypeExample.xlsx&quot;);
            
        }
```

### See Also

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


