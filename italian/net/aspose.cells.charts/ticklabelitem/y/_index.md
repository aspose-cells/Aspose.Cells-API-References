---
title: "TickLabelItem.Y"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabelItem. Coordinate Y dell'elemento Ticklabel come rapporto rispetto all'altezza del grafico"
type: docs
url: /it/net/aspose.cells.charts/ticklabelitem/y/
---
## TickLabelItem.Y property

Coordinate Y dell'elemento Ticklabel come rapporto dell'altezza del grafico.

```csharp
public double Y { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyYDemo
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
            chart.NSeries.Add("B1:B3", true);
            
            // Imposta i dati dell'asse delle categorie usando NSERIES invece di CategoryData
            chart.NSeries.CategoryData = "A1:A3";

            // Calcola il grafico per garantire che le etichette dei tick vengano generate
            chart.Calculate();

            // Ottieni gli elementi delle etichette dei tick dall'asse delle categorie
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = chart.CategoryAxis.TickLabels.TickLabelItems;

            // Dimostra l'uso della proprietà Y aggiungendo forme allineate alle etichette dei tick
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Aggiungi un rettangolo in ogni posizione Y dell'etichetta del tick
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y, // Using the Y property of TickLabelItem
                    item.X + 0.05, // Small width
                    item.Y + 0.02); // Small height
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // Salva la cartella di lavoro
            workbook.Save("TickLabelItemPropertyYDemo_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


