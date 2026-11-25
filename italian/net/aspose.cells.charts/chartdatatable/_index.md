---
title: "Classe ChartDataTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.ChartDataTable. Rappresenta una tabella dati del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

Rappresenta una tabella dati del grafico.

```csharp
public class ChartDataTable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont/) { get; set; } | True se il testo nell'oggetto cambia dimensione del carattere quando le dimensioni dell'oggetto cambiano. Il valore predefinito è True. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode/) { get; set; } | Ottiene e imposta la modalità di visualizzazione dello sfondo |
| [Border](../../aspose.cells.charts/chartdatatable/border/) { get; } | Restituisce un oggetto Border che rappresenta il bordo dell'oggetto |
| [Font](../../aspose.cells.charts/chartdatatable/font/) { get; } | Ottiene un oggetto [`Font`](./font/) che rappresenta l'impostazione del carattere della tabella dati del grafico specificata. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal/) { get; set; } | (**Obsoleto.**) True se la tabella dati del grafico ha bordi orizzontali delle celle |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline/) { get; set; } | (**Obsolete.**) Vero se la tabella dati del grafico ha bordi di contorno |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical/) { get; set; } | (**Obsolete.**) Vero se la tabella dati del grafico ha bordi verticali delle celle |
| [HasHorizontalBorder](../../aspose.cells.charts/chartdatatable/hashorizontalborder/) { get; set; } | Vero se la tabella dati del grafico ha bordi orizzontali delle celle |
| [HasOutlineBorder](../../aspose.cells.charts/chartdatatable/hasoutlineborder/) { get; set; } | Vero se la tabella dati del grafico ha bordi di contorno |
| [HasVerticalBorder](../../aspose.cells.charts/chartdatatable/hasverticalborder/) { get; set; } | Vero se la tabella dati del grafico ha bordi verticali delle celle |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey/) { get; set; } | Vero se la chiave della legenda dell'etichetta dati è visibile. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDataTableDemo
    {
        public static void ChartDataTableExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Ottenere il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunta di valori di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiunta di NSeries (origine dati del grafico) al grafico dall'intervallo di celle "A1" a "B3"
            chart.NSeries.Add("A1:B3", true);

            // Visualizzazione della tabella dati
            chart.ShowDataTable = true;

            // Recupero della tabella dati del grafico
            ChartDataTable chartTable = chart.ChartDataTable;

            // Impostazione delle proprietà della tabella dati del grafico
            chartTable.Font.Color = Color.Red;
            chartTable.AutoScaleFont = true;
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderOutline = true;
            chartTable.ShowLegendKey = false;

            // Salvataggio del file Excel
            workbook.Save("ChartDataTableExample.xlsx");
            workbook.Save("ChartDataTableExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


