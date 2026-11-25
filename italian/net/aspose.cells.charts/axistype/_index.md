---
title: "Enum AxisType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Charts.AxisType. Rappresenta il tipo di asse"
type: docs
url: /it/net/aspose.cells.charts/axistype/
---
## AxisType enumeration

Rappresenta il tipo di asse.

```csharp
public enum AxisType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Category | `0` | Asse delle categorie |
| Value | `1` | Asse dei valori |
| Series | `2` | Asse delle serie |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisTypeDemo
    {
        public static void AxisTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Determina quali assi esistono nel grafico
            bool hasPrimaryCategoryAxis = chart.HasAxis(AxisType.Category, true);
            bool hasSecondaryCategoryAxis = chart.HasAxis(AxisType.Category, false);
            bool hasPrimaryValueAxis = chart.HasAxis(AxisType.Value, true);
            bool hasSecondaryValueAxis = chart.HasAxis(AxisType.Value, false);

            // Restituisci i risultati
            Console.WriteLine("Has Primary Category Axis: " + hasPrimaryCategoryAxis);
            Console.WriteLine("Has Secondary Category Axis: " + hasSecondaryCategoryAxis);
            Console.WriteLine("Has Primary Value Axis: " + hasPrimaryValueAxis);
            Console.WriteLine("Has Secondary Value Axis: " + hasSecondaryValueAxis);

            // Salva la cartella di lavoro
            workbook.Save("AxisTypeExample.xlsx");
            workbook.Save("AxisTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


