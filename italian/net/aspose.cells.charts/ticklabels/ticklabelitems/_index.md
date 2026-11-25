---
title: "TickLabels.TickLabelItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Ottiene le etichette di tick visualizzate dell'asse"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/ticklabelitems/
---
## TickLabels.TickLabelItems property

Ottiene le etichette dei segni di visualizzazione dell'asse.

```csharp
public TickLabelItem[] TickLabelItems { get; }
```

### Osservazioni

Disponibile solo dopo aver chiamato il metodo [`Calculate`](../../chart/calculate/).

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyTickLabelItemsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Calcola il grafico
            chart.Calculate();

            // Ottieni l'asse di categoria e le sue etichette di tick
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Aggiungi forme per contrassegnare la posizione di ogni etichetta di graduazione
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Aggiungi un rettangolo attorno a ogni etichetta di tick
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Transparency = 1;
                shape.Line.SolidFill.Color = Color.Blue;
            }

            // Salva la cartella di lavoro
            workbook.Save("TickLabelItemsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TickLabelItem](../../ticklabelitem/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


