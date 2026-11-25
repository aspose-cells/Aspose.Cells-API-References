---
title: "TickLabelItem.Height"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabelItem. Altezza dell'elemento Ticklabel come rapporto dell'altezza del grafico"
type: docs
url: /it/net/aspose.cells.charts/ticklabelitem/height/
---
## TickLabelItem.Height property

Altezza dell'elemento Ticklabel come rapporto dell'altezza del grafico.

```csharp
public double Height { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyHeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico
            chart.Calculate();

            // Accedi alle etichette di graduazione dell'asse di categoria
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Aggiungi forme per visualizzare le altezze dell'elemento tick label
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Aggiungi rettangolo che mostra i limiti dell'elemento tick label
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Transparency = 1;
                shape.Line.SolidFill.Color = Color.Blue;

                // Aggiungi testo che mostra il valore dell'altezza
                Shape textShape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.TextBox,
                    PlacementType.Move,
                    item.X,
                    item.Y - 0.05, // Position above the tick label
                    0.1,
                    0.05);
                
                textShape.Text = $"H: {item.Height:F4}";
                textShape.Fill.SolidFill.Transparency = 1;
            }

            // Salva la cartella di lavoro
            workbook.Save("TickLabelItemHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


