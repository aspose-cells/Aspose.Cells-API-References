---
title: "Line.DashType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Specifica il tipo di linea tratteggiata"
type: docs
url: /it/net/aspose.cells.drawing/line/dashtype/
---
## Line.DashType property

Specifica il tipo di linea tratteggiata

```csharp
public MsoLineDashStyle DashType { get; set; }
```

### Esempi

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

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Personalizza il tipo di tratteggio della linea della serie
            chart.CategoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;
            chart.CategoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Personalizza la linea della serie
            chart.NSeries[0].Border.DashType = MsoLineDashStyle.Solid;
            chart.NSeries[0].Border.Color = System.Drawing.Color.Blue;

            workbook.Save("LineDashTypeDemo.xlsx");
            Console.WriteLine("Line chart with custom dash types created successfully.");
        }
    }
}
```

### Vedi anche

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


