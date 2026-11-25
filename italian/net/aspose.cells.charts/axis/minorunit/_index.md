---
title: "Axis.MinorUnit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta le unità minori per l'asse"
type: docs
url: /it/net/aspose.cells.charts/axis/minorunit/
---
## Axis.MinorUnit property

Rappresenta le unità secondarie per l'asse.

```csharp
public double MinorUnit { get; set; }
```

### Osservazioni

Le unità minori devono essere maggiori di zero.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorUnitDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Aggiungi dati di esempio
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(70000);
            cells["B3"].PutValue(55000);
            cells["B4"].PutValue(30000);

            // Crea grafico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Configura i dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configura l'asse dei valori
            chart.ValueAxis.Title.Text = "Sales Amount";
            chart.ValueAxis.MajorUnit = 20000;
            chart.ValueAxis.MinorUnit = 5000; // Demonstrate MinorUnit property
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 80000;

            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyMinorUnitDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


