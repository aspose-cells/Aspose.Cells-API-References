---
title: "Enum LineType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.LineType enum. Elenca il tipo di bordo dell'immagine o della linea del grafico"
type: docs
url: /it/net/aspose.cells.drawing/linetype/
---
## LineType enumeration

Elenca il tipo di bordo del [`Picture`](../picture/) o della linea del [`Chart`](../../aspose.cells.charts/chart/).

```csharp
public enum LineType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DarkGray | `6` | Rappresenta una linea grigio scuro. |
| Dash | `1` | Rappresenta una linea tratteggiata. |
| DashDot | `3` | Rappresenta una linea tratto-punto |
| DashDotDot | `4` | Rappresenta una linea tratto-punto-punto. |
| Dot | `2` | Rappresenta una linea puntinata. |
| LightGray | `8` | Rappresenta una linea grigio chiaro. |
| MediumGray | `7` | Rappresenta una linea grigio medio. |
| Solid | `0` | Rappresenta una linea solida. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class LineTypeDemo
    {
        public static void LineTypeExample()
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

            // Accedi all'asse di categoria primario
            Axis categoryAxis = chart.CategoryAxis;

            // Imposta il tipo di linea per la linea dell'asse
            categoryAxis.AxisLine.Style = LineType.DashDot;

            // Imposta il colore della linea dell'asse
            categoryAxis.AxisLine.Color = Color.Blue;

            // Accedi all'asse dei valori primario
            Axis valueAxis = chart.ValueAxis;

            // Imposta il tipo di linea per le linee della griglia principale
            valueAxis.MajorGridLines.Style = LineType.Dot;

            // Imposta il colore delle linee della griglia principale
            valueAxis.MajorGridLines.Color = Color.Red;

            // Salva la cartella di lavoro
            workbook.Save("LineTypeExample.xlsx");

            // Restituisci i risultati
            Console.WriteLine("Chart created with custom line types for axis and gridlines.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


