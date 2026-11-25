---
title: "Chart.Perspective"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Restituisce o imposta la prospettiva per la visualizzazione tridimensionale del grafico. Deve essere compresa tra 0 e 100. Questa proprietà è ignorata se la proprietà RightAngleAxes è True"
type: docs
url: /it/net/aspose.cells.charts/chart/perspective/
---
## Chart.Perspective property

Restituisce o imposta la prospettiva per la visualizzazione tridimensionale del grafico. Deve essere compresa tra 0 e 100. Questa proprietà è ignorata se la proprietà RightAngleAxes è True.

```csharp
public short Perspective { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta le proprietà della prospettiva del grafico 3D
            chart.Perspective = 30; // Perspective angle (0-100)
            chart.RotationAngle = 15; // Rotation angle
            chart.Elevation = 20; // Elevation angle
            chart.RightAngleAxes = false; // Enable perspective projection
            chart.AutoScaling = true; // Auto scale the chart

            // Salva la cartella di lavoro
            workbook.Save("ChartPerspectiveDemo.xlsx");

            Console.WriteLine("Chart with perspective settings created successfully.");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


