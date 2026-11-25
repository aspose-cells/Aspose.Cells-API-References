---
title: "ChartPoint.ShapeX"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 della larghezza del grafico dopo la chiamata al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/shapex/
---
## ChartPoint.ShapeX property

Ottiene la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 della larghezza del grafico dopo aver chiamato il metodo Chart.Calculate().

```csharp
public int ShapeX { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXDemo
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

            // Calcola il grafico per garantire che ShapeX sia popolato
            chart.Calculate();

            // Ottieni il primo punto nella prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore di ShapeX (1/4000 della larghezza del grafico)
            Console.WriteLine("ShapeX value (1/4000 units): " + point.ShapeX);
            Console.WriteLine("ShapeX value (pixels): " + point.ShapeXPx);

            // Dimostra l'uso di ShapeX per posizionare gli elementi rispetto al punto del grafico
            // Nota: Poiché ShapeX è di sola lettura, non possiamo modificarlo direttamente,
            // ma possiamo usarlo per posizionare altri elementi
            if (point.ShapeX > 0)
            {
                // Aggiungi una casella di testo allineata con la posizione X del punto del grafico
                Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(
                    point.ShapeXPx, 100, 100, 50, 100, 50);
                textBox.Text = "Point 1";
            }

            // Salva il risultato
            workbook.Save("ChartPointShapeXDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


