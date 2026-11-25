---
title: "Chart.SideWall"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Restituisce un oggetto Walls che rappresenta la parete laterale di un grafico 3D"
type: docs
url: /it/net/aspose.cells.charts/chart/sidewall/
---
## Chart.SideWall property

Restituisce un oggetto [`Walls`](../walls/) che rappresenta la parete laterale di un grafico 3-D.

```csharp
public Walls SideWall { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertySideWallDemo
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
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:C4", true);

            // Accedi alla proprietà SideWall
            Walls sideWall = chart.SideWall;
            
            // Visualizza alcune proprietà della SideWall
            Console.WriteLine("SideWall properties:");
            Console.WriteLine("Width: " + sideWall.Width);
            Console.WriteLine("Height: " + sideWall.Height);
            Console.WriteLine("Depth: " + sideWall.Depth);

            // Calcola il grafico per aggiornare le dimensioni della parete
            chart.Calculate();

            // Visualizza le proprietà aggiornate dopo il calcolo
            Console.WriteLine("\nAfter Calculate():");
            Console.WriteLine("SideWall CenterX: " + sideWall.CenterX);
            Console.WriteLine("SideWall CenterY: " + sideWall.CenterY);
            Console.WriteLine("SideWall WidthPx: " + sideWall.WidthPx);
            Console.WriteLine("SideWall HeightPx: " + sideWall.HeightPx);

            // Salva la cartella di lavoro
            workbook.Save("ChartPropertySideWallDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


