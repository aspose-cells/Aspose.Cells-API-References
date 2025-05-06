---
title: Axis.MinorUnit
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the minor units for the axis
type: docs
url: /net/aspose.cells.charts/axis/minorunit/
---
## Axis.MinorUnit property

Represents the minor units for the axis.

```csharp
public double MinorUnit { get; set; }
```

### Remarks

The minor units must be greater than zero.

### Examples

```csharp
// Called: chart.CategoryAxis.MinorUnit = 2;
public static void Property_MinorUnit()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            // Adding a new worksheet to the Excel object
            int sheetIndex = workbook.Worksheets.Add();
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Adding sample values to cells
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Dates&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(new DateOnly(2024, 01, 01));
            worksheet.Cells[&quot;A3&quot;].PutValue(new DateOnly(2024, 03, 01));
            worksheet.Cells[&quot;A4&quot;].PutValue(new DateOnly(2024, 05, 01));
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Data1&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(4);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(50);
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Data2&quot;);
            worksheet.Cells[&quot;C2&quot;].PutValue(8);
            worksheet.Cells[&quot;C3&quot;].PutValue(15);
            worksheet.Cells[&quot;C4&quot;].PutValue(30);

            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];
            // Adding NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;B2:C4&quot;, true);

            // Setting the category names for the X-axis from the range &quot;A2:A5&quot;
            chart.NSeries[0].XValues = &quot;A2:A4&quot;;

            // Setting the category axis type to TimeScale
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;

            // Setting the major unit scale for the category axis
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;

            // Setting the minor unit scale for the category axis
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Saving the Excel file
            workbook.Save(&quot;CategoryTypeExample.xlsx&quot;);
            workbook.Save(&quot;CategoryTypeExample.pdf&quot;);

        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


