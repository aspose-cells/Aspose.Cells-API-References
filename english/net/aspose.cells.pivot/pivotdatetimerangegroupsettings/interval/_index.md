---
title: PivotDateTimeRangeGroupSettings.Interval
second_title: Aspose.Cells for .NET API Reference
description: PivotDateTimeRangeGroupSettings property. Gets the internal of the group
type: docs
url: /net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

Gets the internal of the group.

```csharp
public double Interval { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1,groupSettings.Interval);
[Test]
        public void Property_Interval()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
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
            Assert.AreEqual(PivotFieldGroupType.DateTimeRange, groupSettings.Type);

            Assert.AreEqual(1,groupSettings.Interval);
          Assert.IsTrue( groupSettings.IsGroupedBy(PivotGroupByType.Months));
            workbook.Save(Constants.PivotTableDestPath + &quot;CellsNet57018.xlsx&quot;);

        }
```

### See Also

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


