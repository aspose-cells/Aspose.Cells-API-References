---
title: Chart.PivotOptions
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Specifies the pivot controls that appear on the chart
type: docs
url: /net/aspose.cells.charts/chart/pivotoptions/
---
## Chart.PivotOptions property

Specifies the pivot controls that appear on the chart

```csharp
public PivotOptions PivotOptions { get; }
```

### Examples

```csharp
// Called: PivotOptions pivotOptions = chart.PivotOptions;
public static void Property_PivotOptions()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data for the pivot table
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Add a pivot table
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Add a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Access the PivotOptions of the chart
            PivotOptions pivotOptions = chart.PivotOptions;

            // Set properties of PivotOptions
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZoneCategories = true;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZoneSeries = true;
            pivotOptions.DropZonesVisible = true;

            // Save the workbook
            workbook.Save("PivotOptionsExample.xlsx");

            return;
        }
```

### See Also

* class [PivotOptions](../../pivotoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


