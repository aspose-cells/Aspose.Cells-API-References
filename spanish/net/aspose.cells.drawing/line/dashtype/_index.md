---
title: "Line.DashType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Especifica el tipo de línea de guiones"
type: docs
url: /es/net/aspose.cells.drawing/line/dashtype/
---
## Line.DashType property

Especifica el tipo de línea de guiones

```csharp
public MsoLineDashStyle DashType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyDashTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Personalizar el tipo de guión de la línea de la serie
            chart.CategoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;
            chart.CategoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Personalizar la línea de la serie
            chart.NSeries[0].Border.DashType = MsoLineDashStyle.Solid;
            chart.NSeries[0].Border.Color = System.Drawing.Color.Blue;

            workbook.Save("LineDashTypeDemo.xlsx");
            Console.WriteLine("Line chart with custom dash types created successfully.");
        }
    }
}
```

### Ver también

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


