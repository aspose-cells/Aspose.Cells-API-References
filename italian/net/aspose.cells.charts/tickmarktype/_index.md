---
title: "Enum TickMarkType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Charts.TickMarkType. Rappresenta il tipo di segno di spunta per l'asse specificato"
type: docs
url: /it/net/aspose.cells.charts/tickmarktype/
---
## TickMarkType enumeration

Rappresenta il tipo di segno per l'asse specificato.

```csharp
public enum TickMarkType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Cross | `0` | Il tipo di segno di spunta è Cross. |
| Inside | `1` | Il tipo di segno di spunta è Inside. |
| None | `2` | Il tipo di segno di spunta è None. |
| Outside | `3` | Il tipo di segno di spunta è Outside |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickMarkTypeDemo
    {
        public static void TickMarkTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B3"
            chart.NSeries.Add("A1:B3", true);

            // Accedi all'asse dei valori del grafico
            Axis valueAxis = chart.ValueAxis;

            // Imposta il tipo di segno di spunta principale su Cross
            valueAxis.MajorTickMark = TickMarkType.Cross;

            // Imposta il tipo di segno di spunta secondario su Inside
            valueAxis.MinorTickMark = TickMarkType.Inside;

            // Imposta il valore massimo dell'asse dei valori
            valueAxis.MaxValue = 200;

            // Imposta il valore minimo dell'asse dei valori
            valueAxis.MinValue = 0;

            // Imposta l'unità principale
            valueAxis.MajorUnit = 25;

            // Salva la cartella di lavoro
            workbook.Save("TickMarkTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


