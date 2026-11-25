---
title: "Enum MsoLineDashStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.MsoLineDashStyle. Rappresenta lo stile delle linee tratteggiate"
type: docs
url: /it/net/aspose.cells.drawing/msolinedashstyle/
---
## MsoLineDashStyle enumeration

Rappresenta lo stile delle linee tratteggiate.

```csharp
public enum MsoLineDashStyle
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Dash | `0` | Rappresenta una linea tratteggiata. |
| DashDot | `1` | Rappresenta una linea tratto-punto. |
| DashDotDot | `2` | Rappresenta una linea tratto-punto-punto. |
| DashLongDash | `3` | Rappresenta una linea tratto lungo-tratto corto. |
| DashLongDashDot | `4` | Rappresenta una linea tratto lungo-tratto corto-punto. |
| RoundDot | `5` | Rappresenta una linea a punti rotondi. |
| Solid | `6` | Rappresenta una linea solida. |
| SquareDot | `7` | Rappresenta una linea a punti quadrati. |
| Custom | `8` | Stile tratteggio personalizzato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineDashStyleDemo
    {
        public static void MsoLineDashStyleExample()
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

            // Imposta lo stile del tratto delle linee della griglia principale
            categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;

            // Imposta lo stile del tratto delle linee della griglia secondaria
            categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Salva la cartella di lavoro
            workbook.Save("MsoLineDashStyleExample.xlsx");

            // Restituisci i risultati
            Console.WriteLine("Chart with custom dash styles for gridlines created successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


