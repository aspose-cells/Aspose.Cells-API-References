---
title: "Title.Y"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Title. Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/title/y/
---
## Title.Y property

Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use Title.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà Title.YRatioToChart, invece. Y = YRatioToChart * 4000; Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TitlePropertyYDemo
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

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta titolo del grafico
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrating Y property - position in 1/4000 units
            
            // Calcola il grafico per garantire che il layout sia aggiornato
            chart.Calculate();

            // Aggiungi una forma allineata con la posizione Y del titolo
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.Move,
                2000, 
                chart.Title.Y, // Using the title's Y property
                3000, 
                chart.Title.Y + 500);
            shape.Fill.SolidFill.Color = Color.Blue;

            // Salva la cartella di lavoro
            workbook.Save("TitlePropertyYDemo_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


