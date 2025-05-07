---
title: Line.CompoundType
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the compound line type
type: docs
url: /net/aspose.cells.drawing/line/compoundtype/
---
## Line.CompoundType property

Specifies the compound line type

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### Examples

```csharp
// Called: axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
public static void Property_CompoundType()
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

            // Set the line style for the primary category axis
            Line axisLine = categoryAxis.AxisLine;
            axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
            axisLine.Color = Color.Blue;
            axisLine.WeightPt = 2.0;

            // Output the line style
            Console.WriteLine("Axis Line Style: " + axisLine.CompoundType);
            Console.WriteLine("Axis Line Color: " + axisLine.Color);
            Console.WriteLine("Axis Line Weight: " + axisLine.WeightPt);

            // Save the workbook
            workbook.Save("MsoLineStyleExample.xlsx");
        }
```

### See Also

* enum [MsoLineStyle](../../msolinestyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


