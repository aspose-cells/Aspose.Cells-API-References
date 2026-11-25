---
title: "Classe TickLabelItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.TickLabelItem. Rappresenta un'etichetta di graduazione nel grafico"
type: docs
url: /it/net/aspose.cells.charts/ticklabelitem/
---
## TickLabelItem class

Rappresenta un'etichetta di graduazione nel grafico.

```csharp
public class TickLabelItem
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Height](../../aspose.cells.charts/ticklabelitem/height/) { get; } | Altezza dell'elemento Ticklabel come rapporto dell'altezza del grafico. |
| [Width](../../aspose.cells.charts/ticklabelitem/width/) { get; } | Larghezza dell'elemento Ticklabel come rapporto della larghezza del grafico. |
| [X](../../aspose.cells.charts/ticklabelitem/x/) { get; } | Coordinate X dell'elemento Ticklabel come rapporto della larghezza del grafico. |
| [Y](../../aspose.cells.charts/ticklabelitem/y/) { get; } | Coordinate Y dell'elemento Ticklabel come rapporto dell'altezza del grafico. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartsClassTickLabelItemDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico
            chart.Calculate();

            // Accedi alle etichette di graduazione dell'asse di categoria
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Aggiungi forme per contrassegnare la posizione di ogni etichetta di graduazione
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Aggiungi un rettangolo attorno all'etichetta di graduazione
                Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                rectangle.Fill.SolidFill.Transparency = 1;
                rectangle.Line.SolidFill.Color = Color.Blue;

                // Aggiungi un cerchio accanto all'etichetta di graduazione
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + item.Height,
                    item.Y + item.Height);
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Salva la cartella di lavoro
            workbook.Save("TickLabelItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


