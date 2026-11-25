---
title: "Chart.BackWall"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Restituisce un oggetto Walls che rappresenta la parete posteriore di un grafico 3D"
type: docs
url: /it/net/aspose.cells.charts/chart/backwall/
---
## Chart.BackWall property

Restituisce un oggetto [`Walls`](../walls/) che rappresenta la parete posteriore di un grafico 3-D.

```csharp
public Walls BackWall { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyBackWallDemo
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
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Assicurati che sia un grafico 3D
            if (chart.Is3D)
            {
                // Ottieni l'oggetto BackWall
                Walls backWall = chart.BackWall;

                // Visualizza alcune proprietà del BackWall
                Console.WriteLine("BackWall properties:");
                Console.WriteLine("CenterX: " + backWall.CenterX);
                Console.WriteLine("CenterY: " + backWall.CenterY);
                Console.WriteLine("Width: " + backWall.Width);
                Console.WriteLine("Height: " + backWall.Height);

                // Formatta il BackWall
                backWall.FillFormat.SetOneColorGradient(
                    System.Drawing.Color.LightBlue, 
                    0.5, // Changed from GradientStyleType to double for degree parameter
                    Aspose.Cells.Drawing.GradientStyleType.Horizontal, 
                    1); // Changed from 0.5 to int for variant parameter

                // Imposta le proprietà del bordo
                backWall.Border.Color = System.Drawing.Color.DarkBlue;
                backWall.Border.Weight = Aspose.Cells.Drawing.WeightType.MediumLine;
            }

            // Salva la cartella di lavoro
            workbook.Save("ChartPropertyBackWallDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


