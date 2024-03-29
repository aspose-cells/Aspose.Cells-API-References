---
title: ChartDataTable
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta una tabella di dati del grafico.
type: docs
weight: 460
url: /it/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

Rappresenta una tabella di dati del grafico.

```csharp
public class ChartDataTable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont) { get; set; } | Vero se il testo nell'oggetto cambia la dimensione del carattere quando cambia la dimensione dell'oggetto. Il valore predefinito è True. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode) { get; set; } | Ottiene e imposta la modalità di visualizzazione dello sfondo |
| [Border](../../aspose.cells.charts/chartdatatable/border) { get; } | Restituisce un oggetto Border che rappresenta il bordo dell'oggetto |
| [Font](../../aspose.cells.charts/chartdatatable/font) { get; } | Ottiene a[`Font`](./font) oggetto che rappresenta l'impostazione del carattere della tabella dati del grafico specificata. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal) { get; set; } | Vero se la tabella dei dati del grafico ha bordi di celle orizzontali |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline) { get; set; } | Vero se la tabella dei dati del grafico ha bordi di contorno |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical) { get; set; } | Vero se la tabella dei dati del grafico ha bordi di celle verticali |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey) { get; set; } | Vero se la chiave della legenda dell'etichetta dati è visibile. |

### Esempi

```csharp

[C#]

//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();

//Ottenere il riferimento del primo foglio di lavoro
Worksheet worksheet = workbook.Worksheets[0];

//Aggiunta di un valore di esempio alla cella "A1".
worksheet.Cells["A1"].PutValue(50);

//Aggiunta di un valore di esempio alla cella "A2".
worksheet.Cells["A2"].PutValue(100);

//Aggiunta di un valore di esempio alla cella "A3".
worksheet.Cells["A3"].PutValue(150);

//Aggiunta di un valore di esempio alla cella "B1".
worksheet.Cells["B1"].PutValue(60);

//Aggiunta di un valore di esempio alla cella "B2".
worksheet.Cells["B2"].PutValue(32);

//Aggiunta di un valore di esempio alla cella "B3".
worksheet.Cells["B3"].PutValue(50);

//Aggiunta di un grafico al foglio di lavoro
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

//Accesso all'istanza del grafico appena aggiunto
Chart chart = worksheet.Charts[chartIndex];

//Aggiunta di NSeries (origine dati grafico) al grafico che va dalla cella "A1" a "B3"
chart.NSeries.Add("A1:B3", true);

chart.ShowDataTable = true;

//Come ottenere la tabella dei grafici
ChartDataTable chartTable = chart.ChartDataTable;

//Impostazione del colore del carattere della tabella dei grafici
chartTable.Font.Color = System.Drawing.Color.Red;

//Impostazione di Legend Key VisibilityOptions
chartTable.ShowLegendKey = false;

//Salvataggio del file Excel
workbook.Save("book1.xls");

[VB.NET]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()

'Ottenere il riferimento del primo foglio di lavoro
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)

'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)

'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)

'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)

'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)

'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)

'Aggiunta di un grafico al foglio di lavoro
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10)

'Accesso all'istanza del grafico appena aggiunto
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

chart.ShowDataTable = True

'Ottenere la tabella dei grafici
Dim chartTable As ChartDataTable = chart.ChartDataTable

'Impostazione del colore del carattere della tabella dei grafici
chartTable.Font.Color = System.Drawing.Color.Red

'Impostazione delle opzioni di visibilità della chiave della legenda
chartTable.ShowLegendKey = False

'Salvataggio del file Excel
workbook.Save("book1.xls")

```

### Guarda anche

* spazio dei nomi [Aspose.Cells.Charts](../../aspose.cells.charts)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
