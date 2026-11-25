---
title: "Enum FormattingType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.FormattingType enum. Rappresenta il tipo di formattazione applicata a un oggetto Area o a un oggetto Line"
type: docs
url: /it/net/aspose.cells.charts/formattingtype/
---
## FormattingType enumeration

Rappresenta il tipo di formattazione applicata a un oggetto [`Area`](../../aspose.cells.drawing/area/) o a un oggetto [`Line`](../../aspose.cells.drawing/line/).

```csharp
public enum FormattingType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Rappresenta il tipo di formattazione automatica. |
| Custom | `2` | Rappresenta il tipo di formattazione personalizzata. |
| None | `1` | Rappresenta il tipo di formattazione nessuna. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class FormattingTypeDemo
    {
        public static void FormattingTypeExample()
        {
            // Istanzia un oggetto Workbook
            Workbook workbook = new Workbook();
            
            // Aggiungere un nuovo foglio di lavoro all'oggetto Workbook
            int sheetIndex = workbook.Worksheets.Add();
            
            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Aggiunta di valori di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiunta di NSeries (origine dati del grafico) al grafico dall'intervallo di celle "A1" a "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Impostazione del colore di primo piano dell'area del grafico
            chart.PlotArea.Area.ForegroundColor = Color.Blue;
            chart.PlotArea.Area.Formatting = FormattingType.Custom;
            
            // Impostazione del colore di primo piano dell'area del diagramma
            chart.ChartArea.Area.ForegroundColor = Color.Yellow;
            chart.ChartArea.Area.Formatting = FormattingType.Automatic;
            
            // Impostazione del colore di primo piano dell'area della prima NSeries
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.Formatting = FormattingType.None;
            
            // Impostazione del colore di primo piano dell'area del primo punto NSeries
            chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
            chart.NSeries[0].Points[0].Area.Formatting = FormattingType.Custom;
            
            // Salvataggio del file Excel
            workbook.Save("FormattingTypeExample.xlsx");
            workbook.Save("FormattingTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


