---
title: "Axis.CustomUnit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Specifica un valore personalizzato per l'unità di visualizzazione"
type: docs
url: /it/net/aspose.cells.charts/axis/customunit/
---
## Axis.CustomUnit property

Specifica un valore personalizzato per l'unità di visualizzazione.

```csharp
[Obsolete("Use Axis.CustomDisplayUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustomUnit { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà Axis.CustomDisplayUnit. Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustomUnitDemo
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
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Accedi all'asse dei valori
                Axis valueAxis = chart.ValueAxis;

                // Imposta l'unità di visualizzazione su personalizzata
                valueAxis.DisplayUnit = DisplayUnitType.Custom;

                // Imposta il valore dell'unità di visualizzazione personalizzata
                valueAxis.CustomDisplayUnit = 1000000;

                // Visualizza il valore della proprietà CustomUnit (proprietà obsoleta)
                Console.WriteLine("CustomUnit value: " + valueAxis.CustomUnit);

                // Salva la cartella di lavoro
                workbook.Save("AxisPropertyCustomUnitDemo.xlsx");
                Console.WriteLine("CustomUnit has been demonstrated");
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

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


