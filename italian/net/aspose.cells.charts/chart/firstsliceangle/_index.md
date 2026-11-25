---
title: "Chart.FirstSliceAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene o imposta l'angolo della prima fetta di un grafico a torta o a ciambella in gradi in senso orario dalla verticale. Si applica solo ai grafici a torta, a torta 3D e a ciambella da 0 a 360"
type: docs
url: /it/net/aspose.cells.charts/chart/firstsliceangle/
---
## Chart.FirstSliceAngle property

Ottiene o imposta l'angolo della prima fetta di grafico a torta o di ciambella, in gradi (in senso orario dal verticale). Si applica solo a grafici a torta, a torta 3-D e a ciambella, da 0 a 360.

```csharp
public int FirstSliceAngle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Aggiungi grafico a torta
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dei dati
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Imposta l'angolo della prima fetta a 45 gradi
            chart.FirstSliceAngle = 45;
            
            // Salva la cartella di lavoro
            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


