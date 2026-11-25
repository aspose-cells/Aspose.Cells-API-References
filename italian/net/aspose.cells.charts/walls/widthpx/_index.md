---
title: "Walls.WidthPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Walls. Ottiene la larghezza da sinistra a destra in unità di pixel dopo la chiamata al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/walls/widthpx/
---
## Walls.WidthPx property

Ottiene la larghezza da sinistra a destra in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

```csharp
public int WidthPx { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyWidthPxDemo
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

            // Aggiungi grafico 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Ottieni i muri e dimostra la proprietà WidthPx
            Walls walls = chart.Walls;
            Console.WriteLine("Wall width in pixels: " + walls.WidthPx);

            // Salva cartella di lavoro
            workbook.Save("WallsWidthPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


