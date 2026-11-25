---
title: "Enum ChartLineFormattingType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.ChartLineFormattingType enum. Rappresenta il tipo di formato della linea del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartlineformattingtype/
---
## ChartLineFormattingType enumeration

Rappresenta il tipo di formato della linea del grafico.

```csharp
public enum ChartLineFormattingType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Rappresenta il tipo di formattazione automatica. |
| Solid | `1` | Rappresenta il tipo di formattazione solida. |
| None | `2` | Rappresenta il tipo di formattazione nessuna. |
| Gradient | `3` | Gradiente |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartLineFormattingTypeDemo
    {
        public static void ChartLineFormattingTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie al grafico
            chart.NSeries.Add("A1:B3", true);
            
            // Imposta i dati della categoria
            chart.NSeries.CategoryData = "A1:A3";
            
            // Imposta diversi tipi di formattazione della linea per la serie
            chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
            chart.NSeries[0].SeriesLines.Color = Color.Red;
            
            // Aggiungi un'altra serie con formattazione diversa
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
            chart.NSeries[1].SeriesLines.Color = Color.Blue;
            
            // Salva la cartella di lavoro
            workbook.Save("ChartLineFormattingTypeExample.xlsx");
            workbook.Save("ChartLineFormattingTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


