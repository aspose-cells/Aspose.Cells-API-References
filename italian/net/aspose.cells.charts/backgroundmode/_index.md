---
title: "Enum BackgroundMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.BackgroundMode enum. Rappresenta la modalità di visualizzazione dello sfondo"
type: docs
url: /it/net/aspose.cells.charts/backgroundmode/
---
## BackgroundMode enumeration

Rappresenta la modalità di visualizzazione dello sfondo.

```csharp
public enum BackgroundMode
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Automatico |
| Opaque | `1` | Opaco |
| Transparent | `2` | Trasparente |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class BackgroundModeDemo
    {
        public static void BackgroundModeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Accedi all'area del grafico
            ChartArea chartArea = chart.ChartArea;

            // Imposta il colore di primo piano dell'area del grafico
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Imposta la modalità di sfondo dell'area del grafico
            chartArea.BackgroundMode = BackgroundMode.Opaque;
            chartArea.Area.Transparency = 0.8;           
            
            
            // Imposta l'ombra dell'area del grafico
            chartArea.Shadow = true;
            
            // Salva la cartella di lavoro
            workbook.Save("BackgroundModeExample.xlsx");
            workbook.Save("BackgroundModeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


