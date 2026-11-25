---
title: "Chart.WallsAndGridlines2D"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. True se le linee della griglia sono disegnate bidimensionalmente su un grafico 3D"
type: docs
url: /it/net/aspose.cells.charts/chart/wallsandgridlines2d/
---
## Chart.WallsAndGridlines2D property

Vero se le linee della griglia sono disegnate bidimensionalmente su un grafico 3-D.

```csharp
public bool WallsAndGridlines2D { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsAndGridlines2DDemo
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
            worksheet.Cells["B4"].PutValue(15);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Dimostra la proprietà WallsAndGridlines2D
            chart.WallsAndGridlines2D = true; // Show walls and gridlines in 2D
            Console.WriteLine("WallsAndGridlines2D is set to: " + chart.WallsAndGridlines2D);

            // Salva la cartella di lavoro
            workbook.Save("WallsAndGridlines2DDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


