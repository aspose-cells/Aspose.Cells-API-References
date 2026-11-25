---
title: "Enum LineJoinType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.LineJoinType enum. Rappresenta gli stili di giunzione di una linea"
type: docs
url: /it/net/aspose.cells.drawing/linejointype/
---
## LineJoinType enumeration

Rappresenta gli stili di giunzione di una linea.

```csharp
public enum LineJoinType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Round | `0` | Giunzione arrotondata |
| Bevel | `1` | Giunzione smussata |
| Miter | `2` | Giunzione a spigolo |
| None | `3` | Nessuna giunzione |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LineJoinTypeDemo
    {
        public static void LineJoinTypeExample()
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

            // Accedi all'asse dei valori primario
            Axis valueAxis = chart.ValueAxis;

            // Accedi al formato della linea delle griglie principali
            Line majorGridLines = valueAxis.MajorGridLines;

            // Imposta il tipo di giunzione della linea
            majorGridLines.JoinType = LineJoinType.Round;

            // Restituisci il tipo di giunzione
            Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);

            // Salva la cartella di lavoro
            workbook.Save("LineJoinTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


