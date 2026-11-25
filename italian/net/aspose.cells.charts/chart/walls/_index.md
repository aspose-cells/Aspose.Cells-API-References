---
title: "Chart.Walls"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Restituisce un oggetto Walls che rappresenta le pareti di un grafico 3D"
type: docs
url: /it/net/aspose.cells.charts/chart/walls/
---
## Chart.Walls property

Restituisce un oggetto `Walls` che rappresenta le pareti di un grafico 3-D.

```csharp
public Walls Walls { get; }
```

### Osservazioni

Questa proprietà non si applica ai grafici a torta 3-D.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(35);

            // Crea un grafico a colonne cilindrico
            int chartIndex = worksheet.Charts.Add(ChartType.Cylinder, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Configura le impostazioni di base del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.IsRectangularCornered = true;
            chart.RotationAngle = 20;

            // Configura le proprietà delle pareti
            Walls walls = chart.Walls;
            walls.BackgroundColor = Color.LightGray;
            walls.ForegroundColor = Color.Transparent;
            walls.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Horizontal, 1);

            // Salva il risultato
            workbook.Save("ChartWallsDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


