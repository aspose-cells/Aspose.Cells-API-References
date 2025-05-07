---
title: DataLabels.ShapeType
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets or sets shape type of data label
type: docs
url: /net/aspose.cells.charts/datalabels/shapetype/
---
## DataLabels.ShapeType property

Gets or sets shape type of data label.

```csharp
public DataLabelShapeType ShapeType { get; set; }
```

### Examples

```csharp
// Called: series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;
public static void Property_ShapeType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Access the first series in the chart
            Series series = chart.NSeries[0];

            // Enable data labels for the series
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;

            // Save the workbook
            workbook.Save("DataLabelShapeTypeExample.xlsx");
            workbook.Save("DataLabelShapeTypeExample.pdf");
        }
```

### See Also

* enum [DataLabelShapeType](../../../aspose.cells.drawing/datalabelshapetype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


