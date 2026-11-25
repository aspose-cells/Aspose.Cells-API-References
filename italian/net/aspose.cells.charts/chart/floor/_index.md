---
title: "Chart.Floor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Restituisce un oggetto Floor che rappresenta le pareti di un grafico 3D"
type: docs
url: /it/net/aspose.cells.charts/chart/floor/
---
## Chart.Floor property

Restituisce un oggetto `Floor` che rappresenta le pareti di un grafico 3-D.

```csharp
public Floor Floor { get; }
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
    public class ChartPropertyFloorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi e modifica le proprietà del piano
            Floor floor = chart.Floor;
            floor.FillFormat.SetTwoColorGradient(System.Drawing.Color.LightBlue, System.Drawing.Color.DarkBlue, GradientStyleType.Horizontal, 2);
            floor.Border.Color = System.Drawing.Color.Black;

            // Salva la cartella di lavoro
            workbook.Save("ChartFloorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Floor](../../floor/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


