---
title: "ChartPoint.BorderWidthPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la larghezza del bordo in unità di pixel dopo la chiamata al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/borderwidthpx/
---
## ChartPoint.BorderWidthPx property

Ottiene la larghezza del bordo in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

```csharp
public int BorderWidthPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartPointPropertyBorderWidthPxDemo
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
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Aggiungi un grafico e imposta il suo intervallo di dati
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Calcola il grafico per garantire che le proprietà siano popolate
            chart.Calculate();

            // Ottieni il primo punto del grafico nella prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza la larghezza attuale del bordo
            Console.WriteLine("Current BorderWidthPx value: " + point.BorderWidthPx);

            // Nota: BorderWidthPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Invece, possiamo modificare il bordo tramite la proprietà Border
            if (point.Border != null)
            {
                // Modifica la larghezza del bordo impostando il peso usando l'enumerazione WeightType
                point.Border.Weight = WeightType.MediumLine; // Medium weight border
            }

            // Ricalcola per aggiornare il valore di BorderWidthPx
            chart.Calculate();

            // Visualizza la nuova larghezza del bordo in pixel
            Console.WriteLine("New BorderWidthPx value after modification: " + point.BorderWidthPx);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyBorderWidthPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


