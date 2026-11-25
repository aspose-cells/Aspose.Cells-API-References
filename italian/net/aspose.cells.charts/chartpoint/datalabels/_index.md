---
title: "ChartPoint.DataLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Restituisce un oggetto DataLabels che rappresenta l'etichetta dati associata a questo punto del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/datalabels/
---
## ChartPoint.DataLabels property

Restituisce un oggetto `DataLabels` che rappresenta l'etichetta dati associata a questo punto del grafico.

```csharp
public DataLabels DataLabels { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDataLabelsDemo
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

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Accedi al primo punto del grafico
                ChartPoint point = chart.NSeries[0].Points[0];

                // Ottieni la proprietà DataLabels (di sola lettura)
                DataLabels dataLabels = point.DataLabels;

                // Visualizza le proprietà di DataLabels
                Console.WriteLine("DataLabels ShowValue: " + dataLabels.ShowValue);
                Console.WriteLine("DataLabels ShowCategoryName: " + dataLabels.ShowCategoryName);
                Console.WriteLine("DataLabels ShowSeriesName: " + dataLabels.ShowSeriesName);
                Console.WriteLine("DataLabels Position: " + dataLabels.Position);

                // Modifica alcune proprietà di DataLabels (poiché DataLabels non è di sola lettura)
                dataLabels.ShowValue = true;
                dataLabels.ShowCategoryName = true;
                dataLabels.Position = LabelPositionType.OutsideEnd;

                // Salva il risultato
                workbook.Save("ChartPointDataLabelsDemo.xlsx");
                Console.WriteLine("DataLabels demonstration completed successfully.");
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

* class [DataLabels](../../datalabels/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


