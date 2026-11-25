---
title: "Walls.Width"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Walls. Ottiene la larghezza da sinistra a destra in unità di 1/4000 della larghezza del grafico dopo le chiamate al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/walls/width/
---
## Walls.Width property

Ottiene la larghezza da sinistra a destra in unità di 1/4000 della larghezza del grafico dopo le chiamate al metodo Chart.Calculate().

```csharp
public int Width { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyWidthDemo
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

            // Aggiungi un grafico 3D
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico
            chart.Calculate();

            // Accedi ai muri e dimostra la proprietà Width
            Aspose.Cells.Charts.Walls walls = chart.Walls;
            Console.WriteLine("Wall Width: " + walls.Width);
            Console.WriteLine("Wall Width in Pixels: " + walls.WidthPx);

            // Salva la cartella di lavoro
            workbook.Save("WallsWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


