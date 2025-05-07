---
title: Line.DashType
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the dash line type
type: docs
url: /net/aspose.cells.drawing/line/dashtype/
---
## Line.DashType property

Specifies the dash line type

```csharp
public MsoLineDashStyle DashType { get; set; }
```

### Examples

```csharp
// Called: categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;
public static void Property_DashType()
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

            // Access the primary category axis
            Axis categoryAxis = chart.CategoryAxis;

            // Set the dash style of the major gridlines
            categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;

            // Set the dash style of the minor gridlines
            categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Save the workbook
            workbook.Save("MsoLineDashStyleExample.xlsx");

            // Output the results
            Console.WriteLine("Chart with custom dash styles for gridlines created successfully.");
        }
```

### See Also

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


