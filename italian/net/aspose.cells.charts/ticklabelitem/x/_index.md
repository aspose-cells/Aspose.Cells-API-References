---
title: "TickLabelItem.X"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabelItem. Coordinate X dell'elemento Ticklabel come rapporto rispetto alla larghezza del grafico"
type: docs
url: /it/net/aspose.cells.charts/ticklabelitem/x/
---
## TickLabelItem.X property

Coordinate X dell'elemento Ticklabel come rapporto della larghezza del grafico.

```csharp
public double X { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyXDemo
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

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico
            chart.Calculate();

            // Accedi agli elementi delle etichette dei tick
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] items = axis.TickLabels.TickLabelItems;

            // Aggiungi forme in ogni posizione dell'etichetta del tick usando la proprietà X
            for (int i = 0; i < items.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = items[i];
                
                // Aggiungi un rettangolo nella posizione dell'etichetta del tick
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X, 
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Color = Color.LightBlue;
                shape.Line.SolidFill.Color = Color.Blue;

                // Aggiungi un cerchio accanto all'etichetta del tick usando la proprietà X
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + 0.05, // Small offset
                    item.Y + item.Height);
                
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Salva la cartella di lavoro
            workbook.Save("TickLabelItemPropertyXDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


