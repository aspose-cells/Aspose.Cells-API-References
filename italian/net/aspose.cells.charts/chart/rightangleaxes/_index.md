---
title: "Chart.RightAngleAxes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. True se gli assi del grafico sono perpendicolari. Si applica solo ai grafici 3D, eccetto Column3D e 3D Pie Charts"
type: docs
url: /it/net/aspose.cells.charts/chart/rightangleaxes/
---
## Chart.RightAngleAxes property

Vero se gli assi del grafico sono perpendicolari. Si applica solo ai grafici 3-D (eccetto Column3D e grafici a torta 3-D).

```csharp
public bool RightAngleAxes { get; set; }
```

### Osservazioni

Se questa proprietà è True, la proprietà Perspective viene ignorata.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRightAngleAxesDemo
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
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Dimostra la proprietà RightAngleAxes
            chart.RightAngleAxes = true;
            Console.WriteLine("RightAngleAxes is set to: " + chart.RightAngleAxes);

            // Salva la cartella di lavoro
            workbook.Save("RightAngleAxesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


