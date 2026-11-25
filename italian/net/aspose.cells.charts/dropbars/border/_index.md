---
title: "DropBars.Border"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DropBars. Ottiene la Linea del bordo"
type: docs
url: /it/net/aspose.cells.charts/dropbars/border/
---
## DropBars.Border property

Ottiene il bordo [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsPropertyBorderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi un grafico a linee
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie di dati al grafico
            chart.NSeries.Add("A1:B3", true);

            // Abilita le barre su/giù
            chart.NSeries[0].HasUpDownBars = true;

            try
            {
                // Accedi agli oggetti DropBars
                DropBars upBars = chart.NSeries[0].UpBars;
                DropBars downBars = chart.NSeries[0].DownBars;

                // Visualizza le proprietà del bordo attuali (accesso in sola lettura)
                Console.WriteLine("Up Bars Border Color: " + upBars.Border.Color);
                Console.WriteLine("Up Bars Border Style: " + upBars.Border.Style);
                Console.WriteLine("Up Bars Border Weight: " + upBars.Border.WeightPt);
                Console.WriteLine("Up Bars Border Visibility: " + upBars.Border.IsVisible);

                Console.WriteLine("\nDown Bars Border Color: " + downBars.Border.Color);
                Console.WriteLine("Down Bars Border Style: " + downBars.Border.Style);
                Console.WriteLine("Down Bars Border Weight: " + downBars.Border.WeightPt);
                Console.WriteLine("Down Bars Border Visibility: " + downBars.Border.IsVisible);

                // Modifica le proprietà del bordo (poiché Line non è in sola lettura)
                upBars.Border.Color = Color.Blue;
                upBars.Border.Style = LineType.Solid;
                upBars.Border.WeightPt = 2.0;
                upBars.Border.IsVisible = true;

                downBars.Border.Color = Color.Red;
                downBars.Border.Style = LineType.Dash;
                downBars.Border.WeightPt = 1.5;
                downBars.Border.IsVisible = true;

                // Salva la cartella di lavoro
                workbook.Save("DropBarsBorderDemo.xlsx");
                Console.WriteLine("\nBorder properties have been demonstrated and saved to file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Line](../../../aspose.cells.drawing/line/)
* class [DropBars](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


