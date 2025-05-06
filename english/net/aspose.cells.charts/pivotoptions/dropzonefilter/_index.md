---
title: PivotOptions.DropZoneFilter
second_title: Aspose.Cells for .NET API Reference
description: PivotOptions property. Specifies whether a control for each PivotTable field on the PivotTable page axis of the source PivotTable appears on the chart when dropZonesVisible is set to true
type: docs
url: /net/aspose.cells.charts/pivotoptions/dropzonefilter/
---
## PivotOptions.DropZoneFilter property

Specifies whether a control for each PivotTable field on the PivotTable page axis of the source PivotTable appears on the chart when dropZonesVisible is set to true.

```csharp
public bool DropZoneFilter { get; set; }
```

### Examples

```csharp
// Called: pivotOptions.DropZoneFilter = true;
public static void Property_DropZoneFilter()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data for the pivot table
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);
            worksheet.Cells[&quot;A5&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;B5&quot;].PutValue(40);

            // Add a pivot table
            int pivotIndex = worksheet.PivotTables.Add(&quot;=A1:B5&quot;, &quot;D1&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Add a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = &quot;PivotTable1&quot;;

            // Access the PivotOptions of the chart
            PivotOptions pivotOptions = chart.PivotOptions;

            // Set properties of PivotOptions
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZoneCategories = true;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZoneSeries = true;
            pivotOptions.DropZonesVisible = true;

            // Save the workbook
            workbook.Save(&quot;PivotOptionsExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


